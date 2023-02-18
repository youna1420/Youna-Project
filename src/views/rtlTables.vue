<template>
    <div class="py-4 container-fluid">
    <div class="row">
      <div class="col-12">
        <authors-table />
      </div>
    </div>
  </div>
  </template>
  
  <script>
  /* eslint-disable */ 
  import MiniStatisticsCard from "@/examples/Cards/MiniStatisticsCard.vue";
  import ReportsBarChart from "@/examples/Charts/ReportsBarChart";
  import GradientLineChart from "@/examples/Charts/GradientLineChart.vue";
  import TimelineList from "./components/TimelineList.vue";
  import AuthorsTable from "./components/AuthorsTable";
  import ProjectsTable from "./components/ProjectsTable";
  import setTooltip from "@/assets/js/tooltip.js";
  import {
    faHandPointer,
    faUsers,
    faCreditCard,
    faScrewdriverWrench,
  } from "@fortawesome/free-solid-svg-icons";
  
  export default {
    name: "rtl-page",
    data() {
      return {
        iconBackground: "bg-gradient-success",
        faHandPointer,
        faUsers,
        faCreditCard,
        faScrewdriverWrench,
      };
    },
    components: {
      MiniStatisticsCard,
      ReportsBarChart,
      GradientLineChart,
      TimelineList,
      AuthorsTable,
      ProjectsTable
    },
    mounted() {
      setTooltip();
    },
    beforeMount() {
      this.$store.state.isRTL = true;
      document.querySelector("html").setAttribute("lang", "ar");
      document.querySelector("html").setAttribute("dir", "rtl");
      document.querySelector("#app").classList.add("rtl");
    },
    beforeUnmount() {
      this.$store.state.isRTL = false;
      document.querySelector("html").removeAttribute("lang");
      document.querySelector("html").removeAttribute("dir");
      document.querySelector("#app").classList.remove("rtl");
    },
  };
  </script>
  