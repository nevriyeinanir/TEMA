<template>

<div>
    <div>Index: {{ index }}</div>
    <div>Names Array: {{ name }}</div>
  </div>

    <div class="row row-deck row-cards" >
            <div class="col-sm-6 col-lg-3">
              <div class="card">
                <div class="card-body">
                  <div class="d-flex align-items-center">
                    <div class="subheader">{{name}}</div>
                    <div class="ms-auto lh-1">
                      <div class="dropdown">
                        <a class="dropdown-toggle text-muted" href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Last 7 days</a>
                        <div class="dropdown-menu dropdown-menu-end">
                          <a class="dropdown-item active" href="#">Last 7 days</a>
                          <a class="dropdown-item" href="#">Last 30 days</a>
                          <a class="dropdown-item" href="#">Last 3 months</a>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="h1 mb-3">75%</div>
                  <div class="d-flex mb-2">
                    <div>Conversion rate</div>
                    <div class="ms-auto">
                      <span class="text-green d-inline-flex align-items-center lh-1">
                        7% <svg xmlns="http://www.w3.org/2000/svg" class="icon ms-1" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><polyline points="3 17 9 11 13 15 21 7" /><polyline points="14 7 21 7 21 14" /></svg>
                      </span>
                    </div>
                  </div>
                         <div class="progress progress-sm">
                           
                    <div class="progress-bar bg-blue" style="width: 75%" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
                      
                      <span class="visually-hidden">75% Complete</span>
                    </div>
                  </div>
              </div>
              </div>
            </div>
            
  <!--           <div>
  <ApexCharts width="500" type="bar" :options="options" :series="series">
</div>-->
<div class="row row-cards">
<div class="col-12">
<div class="card">
<div class="card-body">
<div class="d-flex">
<h3 class="card-title">Social referrals</h3>
<div class="ms-auto">
<div class="dropdown">
<a class="dropdown-toggle text-muted" href="#" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Last 7 days</a>
<div class="dropdown-menu dropdown-menu-end">
<a class="dropdown-item active" href="#">Last 7 days</a>
<a class="dropdown-item" href="#">Last 30 days</a>
<a class="dropdown-item" href="#">Last 3 months</a>
</div>
</div>
</div>
</div>

<div id="chart-social-referrals"></div>-
</div>---
</div>
</div>
  </div>
  </div>
</template>
<script>
import ApexCharts from 'apexcharts'
export default {
  props: ["name", "index"],
};

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-social-referrals"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 192,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Facebook",
          data: [
            13281,
            8521,
            15038,
            9983,
            15417,
            8888,
            7052,
            14270,
            5214,
            9587,
            5950,
            16852,
            17836,
            12217,
            17406,
            12262,
            9147,
            14961,
            18292,
            15230,
            13435,
            10649,
            5140,
            13680,
            4508,
            13271,
            13413,
            5543,
            18727,
            18238,
            18175,
            6246,
            5864,
            17847,
            9170,
            6445,
            12945,
            8142,
            8980,
            10422,
            15535,
            11569,
            10114,
            17621,
            16138,
            13046,
            6652,
            9906,
            14100,
            16495,
            6749,
          ],
        },
        {
          name: "Twitter",
          data: [
            3680,
            1862,
            3070,
            2252,
            5348,
            3091,
            3000,
            3984,
            5176,
            5325,
            2420,
            5474,
            3098,
            1893,
            3748,
            2879,
            4197,
            5186,
            4213,
            4334,
            2807,
            1594,
            4863,
            2030,
            3752,
            4856,
            5341,
            3954,
            3461,
            3097,
            3404,
            4949,
            2283,
            3227,
            3630,
            2360,
            3477,
            4675,
            1901,
            2252,
            3347,
            2954,
            5029,
            2079,
            2830,
            3292,
            4578,
            3401,
            4104,
            3749,
            4457,
            3734,
          ],
        },
        {
          name: "Dribbble",
          data: [
            722,
            1866,
            961,
            1108,
            1110,
            561,
            1753,
            1815,
            1985,
            776,
            859,
            547,
            1488,
            766,
            702,
            621,
            1599,
            1372,
            1620,
            963,
            759,
            764,
            739,
            789,
            1696,
            1454,
            1842,
            734,
            551,
            1689,
            1924,
            1875,
            908,
            1675,
            1541,
            1953,
            534,
            502,
            1524,
            1867,
            719,
            1472,
            1608,
            1025,
            889,
            1150,
            654,
            1695,
            1662,
            1285,
            1787,
          ],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
        xaxis: {
          lines: {
            show: true,
          },
        },
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
        "2020-06-27",
        "2020-06-28",
        "2020-06-29",
        "2020-06-30",
        "2020-07-01",
        "2020-07-02",
        "2020-07-03",
        "2020-07-04",
        "2020-07-05",
        "2020-07-06",
        "2020-07-07",
        "2020-07-08",
        "2020-07-09",
        "2020-07-10",
        "2020-07-11",
        "2020-07-12",
        "2020-07-13",
        "2020-07-14",
        "2020-07-15",
        "2020-07-16",
        "2020-07-17",
        "2020-07-18",
        "2020-07-19",
        "2020-07-20",
        "2020-07-21",
        "2020-07-22",
        "2020-07-23",
        "2020-07-24",
        "2020-07-25",
        "2020-07-26",
        "2020-07-27",
        "2020-07-28",
        "2020-07-29",
        "2020-07-30",
        "2020-07-31",
        "2020-08-01",
        "2020-08-02",
        "2020-08-03",
        "2020-08-04",
        "2020-08-05",
        "2020-08-06",
        "2020-08-07",
        "2020-08-08",
        "2020-08-09",
      ],
      colors: ["#3b5998", "#1da1f2", "#ea4c89"],
      legend: {
        show: true,
        position: "bottom",
        height: 32,
        offsetY: 8,
        markers: {
          width: 8,
          height: 8,
          radius: 100,
        },
        itemMargin: {
          horizontal: 8,
        },
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-tasks-overview"), {
      chart: {
        type: "bar",
        fontFamily: "inherit",
        height: 320,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      plotOptions: {
        bar: {
          columnWidth: "50%",
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "A",
          data: [
            44,
            32,
            48,
            72,
            60,
            16,
            44,
            32,
            78,
            50,
            68,
            34,
            26,
            48,
            72,
            60,
            84,
            64,
            74,
            52,
            62,
            50,
            32,
            22,
          ],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        categories: [
          "Sprint 1",
          "Sprint 2",
          "Sprint 3",
          "Sprint 4",
          "Sprint 5",
          "Sprint 6",
          "Sprint 7",
          "Sprint 8",
          "Sprint 9",
          "Sprint 10",
          "Sprint 11",
          "Sprint 12",
          "Sprint 13",
          "Sprint 14",
          "Sprint 15",
          "Sprint 16",
          "Sprint 17",
          "Sprint 18",
          "Sprint 19",
          "Sprint 20",
          "Sprint 21",
          "Sprint 22",
          "Sprint 23",
          "Sprint 24",
        ],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks"), {
      chart: {
        type: "bar",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      plotOptions: {
        bar: {
          columnWidth: "50%",
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks2"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks3"), {
      chart: {
        type: "area",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 0.16,
        type: "solid",
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks4"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "straight",
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks5"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "stepline",
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks6"), {
      chart: {
        type: "bar",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      plotOptions: {
        bar: {
          barHeight: "50%",
          horizontal: true,
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks7"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Tasks completion",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks8"), {
      chart: {
        type: "bar",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      plotOptions: {
        bar: {
          columnWidth: "50%",
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
        {
          name: "",
          data: [113, 42, 65, 54, 76, 65, 35],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4", "#cd201f"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks9"), {
      chart: {
        type: "bar",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
        stacked: true,
      },
      plotOptions: {
        bar: {
          columnWidth: "50%",
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
        {
          name: "",
          data: [113, 42, 65, 54, 76, 65, 35],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4", "#cd201f"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks10"), {
      chart: {
        type: "area",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 0.16,
        type: "solid",
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
        {
          name: "",
          data: [113, 42, 65, 54, 76, 65, 35],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4", "#cd201f"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-completion-tasks11"), {
      chart: {
        type: "area",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
        stacked: true,
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 0.16,
        type: "solid",
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "",
          data: [155, 65, 465, 265, 225, 325, 80],
        },
        {
          name: "",
          data: [113, 42, 65, 54, 76, 65, 35],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        type: "datetime",
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      labels: [
        "2020-06-20",
        "2020-06-21",
        "2020-06-22",
        "2020-06-23",
        "2020-06-24",
        "2020-06-25",
        "2020-06-26",
      ],
      colors: ["#206bc4", "#cd201f"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-total-sales"), {
      chart: {
        type: "donut",
        fontFamily: "inherit",
        height: 240,
        sparkline: {
          enabled: true,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      series: [44, 55, 12, 2],
      labels: ["Direct", "Affilliate", "E-mail", "Other"],
      grid: {
        strokeDashArray: 4,
      },
      colors: ["#206bc4", "#79a6dc", "#bfe399", "#e9ecf1"],
      legend: {
        show: false,
      },
      tooltip: {
        fillSeriesColor: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-tasks"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "New",
          data: [0, 0, 1, 2, 21, 9, 12, 10, 31, 13, 65, 10, 12, 6, 4, 3, 0],
        },
        {
          name: "Completed",
          data: [0, 0, 1, 2, 7, 5, 6, 8, 24, 7, 12, 5, 6, 3, 2, 2, 0],
        },
        {
          name: "Closed",
          data: [0, 0, 1, 0, 2, 0, 1, 0, 2, 3, 0, 2, 3, 2, 1, 0, 0],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        categories: [
          "M",
          "T",
          "W",
          "T",
          "F",
          "S",
          "S",
          "M",
          "T",
          "W",
          "T",
          "F",
          "S",
          "S",
          "M",
          "T",
          "W",
        ],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#94d82d", "#ff922b"],
      legend: {
        show: false,
      },
      tooltip: {
        enabled: false,
      },
      point: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-line-stroke"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "straight",
      },
      series: [
        {
          name: "Development",
          data: [8, 10, 11, 12, 20, 27, 30],
        },
        {
          name: "Marketing",
          data: [3, 16, 17, 19, 20, 30, 30],
        },
        {
          name: "Sales",
          data: [7, 10, 11, 18, 18, 18, 24],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        categories: ["2013", "2014", "2015", "2016", "2017", "2018", "2019"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#ff922b", "#206bc4", "#5eba00"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-stepline"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "stepline",
      },
      series: [
        {
          name: "Development",
          data: [34, 44, 54, 21, 12, 43, 33, 23, 66, 66, 58],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#ff922b"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-temperature"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Tokyo",
          data: [
            7.0,
            6.9,
            9.5,
            14.5,
            18.4,
            21.5,
            25.2,
            26.5,
            23.3,
            18.3,
            13.9,
            9.6,
          ],
        },
        {
          name: "London",
          data: [
            3.9,
            4.2,
            5.7,
            8.5,
            11.9,
            15.2,
            17.0,
            16.6,
            14.2,
            10.3,
            6.6,
            4.8,
          ],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      dataLabels: {
        enabled: true,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        categories: [
          "Jan",
          "Feb",
          "Mar",
          "Apr",
          "May",
          "Jun",
          "Jul",
          "Aug",
          "Sep",
          "Oct",
          "Nov",
          "Dec",
        ],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#5eba00"],
      legend: {
        show: false,
      },
      markers: {
        size: 2,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-area"), {
      chart: {
        type: "area",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 0.16,
        type: "solid",
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Maximum",
          data: [11, 8, 15, 18, 19, 17],
        },
        {
          name: "Minimum",
          data: [7, 7, 5, 7, 9, 12],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        categories: ["Jan", "Feb", "Mar", "Apr", "May", "Jun"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#f66d9b"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-area-spline"), {
      chart: {
        type: "area",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 0.16,
        type: "solid",
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Maximum",
          data: [11, 8, 15, 18, 19, 17],
        },
        {
          name: "Minimum",
          data: [7, 7, 5, 7, 9, 12],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        categories: ["Jan", "Feb", "Mar", "Apr", "May", "Jun"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#f66d9b"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-area-spline-stacked"), {
      chart: {
        type: "area",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
        stacked: true,
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 0.16,
        type: "solid",
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Maximum",
          data: [11, 8, 15, 18, 19, 17],
        },
        {
          name: "Minimum",
          data: [7, 7, 5, 7, 9, 12],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        categories: ["Jan", "Feb", "Mar", "Apr", "May", "Jun"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#f66d9b"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-spline"), {
      chart: {
        type: "line",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      stroke: {
        width: 2,
        lineCap: "round",
        curve: "smooth",
      },
      series: [
        {
          name: "Hestavollane",
          data: [
            0.2,
            0.8,
            0.8,
            0.8,
            1,
            1.3,
            1.5,
            2.9,
            1.9,
            2.6,
            1.6,
            3,
            4,
            3.6,
            4.5,
            4.2,
            4.5,
            4.5,
            4,
            3.1,
            2.7,
            4,
            2.7,
            2.3,
            2.3,
            4.1,
            7.7,
            7.1,
            5.6,
            6.1,
            5.8,
            8.6,
            7.2,
            9,
            10.9,
            11.5,
            11.6,
            11.1,
            12,
            12.3,
            10.7,
            9.4,
            9.8,
            9.6,
            9.8,
            9.5,
            8.5,
            7.4,
            7.6,
          ],
        },
        {
          name: "Vik",
          data: [
            0,
            0,
            0.6,
            0.9,
            0.8,
            0.2,
            0,
            0,
            0,
            0.1,
            0.6,
            0.7,
            0.8,
            0.6,
            0.2,
            0,
            0.1,
            0.3,
            0.3,
            0,
            0.1,
            0,
            0,
            0,
            0.2,
            0.1,
            0,
            0.3,
            0,
            0.1,
            0.2,
            0.1,
            0.3,
            0.3,
            0,
            3.1,
            3.1,
            2.5,
            1.5,
            1.9,
            2.1,
            1,
            2.3,
            1.9,
            1.2,
            0.7,
            1.3,
            0.4,
            0.3,
          ],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        categories: ["Jan", "Feb", "Mar", "Apr", "May", "Jun"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#5eba00"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-scatter"), {
      chart: {
        type: "scatter",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "Maximum",
          data: [11, 8, 15, 18, 19, 17],
        },
        {
          name: "Minimum",
          data: [7, 7, 5, 7, 9, 12],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        categories: ["Jan", "Feb", "Mar", "Apr", "May", "Jun"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#206bc4", "#f66d9b"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on

// @formatter:off
document.addEventListener("DOMContentLoaded", function () {
  window.ApexCharts &&
    new ApexCharts(document.getElementById("chart-combination"), {
      chart: {
        type: "bar",
        fontFamily: "inherit",
        height: 240,
        parentHeightOffset: 0,
        toolbar: {
          show: false,
        },
        animations: {
          enabled: false,
        },
      },
      plotOptions: {
        bar: {
          columnWidth: "50%",
        },
      },
      dataLabels: {
        enabled: false,
      },
      fill: {
        opacity: 1,
      },
      series: [
        {
          name: "Development",
          data: [30, 20, 50, 40, 60, 50],
        },
        {
          name: "Marketing",
          data: [200, 130, 90, 240, 130, 220],
        },
        {
          name: "Sales",
          data: [300, 200, 160, 400, 250, 250],
        },
        {
          name: "Sales",
          data: [200, 130, 90, 240, 130, 220],
        },
      ],
      grid: {
        padding: {
          top: -20,
          right: 0,
          left: -4,
          bottom: -4,
        },
        strokeDashArray: 4,
      },
      xaxis: {
        labels: {
          padding: 0,
        },
        tooltip: {
          enabled: false,
        },
        axisBorder: {
          show: false,
        },
        categories: ["2013", "2014", "2015", "2016", "2017", "2018"],
      },
      yaxis: {
        labels: {
          padding: 4,
        },
      },
      colors: ["#5eba00", "#f66d9b", "#5eba00", "#206bc4"],
      legend: {
        show: false,
      },
    }).render();
});
// @formatter:on
</script>