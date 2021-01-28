<!-- Use preprocessors via the lang attribute! e.g. <template lang="pug"> -->
<template>
  <div id="app">
    <button @click="buildWithData">Build data</button>
    <button @click="buildWithoutData">Build without data</button>
    <apexchart
      width="500"
      type="bar"
      :options="chartOptions"
      :series="series"
      ref="chart"
    ></apexchart>
  </div>
</template>

<script>
//Vue.use(VueApexCharts);
import VueApexCharts from 'apexcharts'
export default {
  components: {
    apexchart: VueApexCharts
  },
  data() {
    return {
      series: [],
      chartOptions: {
        chart: {
          type: "bar",
          stacked: true
        },
        dataLabels: {
          enabled: false
        },
        grid: {
          row: {
            colors: ["#fff", "#f2f2f2"]
          }
        },
        xaxis: {
          labels: {
            rotate: -45 //will rotate if label to long
          },
          categories: [],
          tickPlacement: "on"
        },
        fill: {
          type: "gradient",
          gradient: {
            shade: "light",
            type: "horizontal"
          }
        }
      }
    };
  },
  created() {
    this.buildWithData();
  },
  methods: {
    buildWithData() {
      let series = [
        { name: "data 1", data: [1800, 0], groupColor: "#ffd966" },
        { name: "data 2", data: [0, 600], groupColor: "#93c47d" }
      ];
      let categories = ["2020-08-10", "2020-08-15"];
      this._buildGraphic(series, categories);
    },
    buildWithoutData() {
       this._buildGraphic([], []);
    },
    _buildGraphic(series, categories) {
      this.series = series;
      const ext = this;
      this.chartOptions = {
        chart: {
          type: "bar",
          height: 350,
          stacked: true,
          events: {
            mounted: (chartContext, config) => {
              setTimeout(() => {
                this.addAnnotations(config, categories, this);
              });
            },
            updated: (chartContext, config) => {
              setTimeout(() => {
                this.addAnnotations(config, categories, this);
              });
            }
          }
        },
        xaxis: {
          labels: {
            rotate: -45 //will rotate if label to long
          },
          categories: categories
        }
      };
      const colors = series.map((x) => x.groupColor);
      if (colors.length > 0) {
        this.chartOptions.colors = colors;
      }
    },
    addAnnotations(config, categories, vm) {
      const seriesTotals = config.globals.stackedSeriesTotals;

      vm.totalAll = 0;
      if (seriesTotals.length > 0) {
        vm.$refs.chart.clearAnnotations();
        categories.forEach((category, index) => {

          if (seriesTotals[index] > 0) {
            vm.totalAll += seriesTotals[index];

            vm.$refs.chart.addPointAnnotation({
              x: category,
              y: seriesTotals[index],
              label: {
                text: `${seriesTotals[index]}`
              }
            });
          }
        });
      }
    }
  }
};
</script>

<!-- Use preprocessors via the lang attribute! e.g. <style lang="scss"> -->
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

a,
button {
  color: #4fc08d;
}

button {
  background: none;
  border: solid 1px;
  border-radius: 2em;
  font: inherit;
  padding: 0.75em 2em;
}
</style>
