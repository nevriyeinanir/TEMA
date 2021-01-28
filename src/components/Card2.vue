<template>

    <div>Index: {{ index }}</div>
    <div>Names Array: {{ name }}</div>
    <div>Type: {{ typeChart }}</div>
    <div>chartoption: {{ chartoption }}</div>
 <apexcharts
      width="350"
      type="bar"
      :options="chartoption"
      :series="name"
    ></apexcharts>
</template>

<script>
//import VueApexCharts from 'vue-apexcharts'
import VueApexCharts from "vue3-apexcharts";
export default {
  props: ["name", "index", "typeChart"],
  name: "Chart",
chartoption:"",
  components: {
    apexcharts: VueApexCharts,
  },
  data: function () {
    return {
      chartoption:{},
      chartOptions: {
        chart: {
          id: "basic-bar",
        },
        xaxis: {
          categories: [1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998],
        },
      },
      series: [
        {
          name: "series-1",
          data: [30, 40, 45, 50, 49, 60, 70, 91],
        },
      ],
      chartOptionsArea: {
        chart: {
          id: "basic-bar2",
        },
        xaxis: {
          categories: [1, 2, 3, 4, 5, 6, 7, 8],
        },
      },
      series2: [
        {  name: "series-2",
          data: [30, 40, 45, 50, 49, 60, 70, 91],
        },
      ],
    };
  },
  created() {
  if (this.typeChart == "a") {
      this.chartoption = "chartOptions";
    }
    if (this.typeChart == "b") {
      this.chartoption = "chartOptionsArea";
    }
  
  if (this.typeChart == "c") {
      this.chartoption = "chartOptionsArea";
    }
  
}
};
</script>