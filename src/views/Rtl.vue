<template>
  <div class="py-4 container-fluid">
    <div class="row">
      <div class="col-lg-3 col-sm-6 mb-lg-0 mb-4">
        <mini-statistics-card
          title="ارزش کل کالای دپو"
          value="$ 5500"
          :percentage="{
            value: '+55%',
            color: 'text-success',
          }"
          :icon="{
            component: 'ni ni-money-coins',
            background: iconBackground,
          }"
          direction-reverse
        />
      </div>
      <div class="col-lg-3 col-sm-6 mb-lg-0 mb-4">
        <mini-statistics-card
          title="لیست فروشندگان"
          value="نمایش"
          :percentage="{
            value: '+3%',
            color: 'text-success',
          }"
          :icon="{
            component: 'ni ni-world',
            background: iconBackground,
          }"
          direction-reverse
        />
      </div>
      <div class="col-lg-3 col-sm-6 mb-lg-0 mb-4">
        <mini-statistics-card
          title="تعداد کل کالا ها"
          value="+85"
          :percentage="{
            value: '+2%',
            color: 'text-danger',
          }"
          :icon="{
            component: 'ni ni-paper-diploma',
            background: iconBackground,
          }"
          direction-reverse
        />
      </div>
      <div class="col-lg-3 col-sm-6">
        <mini-statistics-card
          title="حجم کالای موجود"
          value="7000 تن"
          :percentage="{
            value: '+5%',
            color: 'text-success',
          }"
          :icon="{
            component: 'ni ni-cart',
            background: iconBackground,
          }"
          direction-reverse
        />
      </div>
    </div>
    <div class="row">
      <div class="col-lg-7 mb-lg-0 mb-4">
        <div class="card">
          <div class="card-body p-3">
            <div class="row">
              <div class="col-lg-6 mb-lg-0 mb-4">
                <div class="d-flex flex-column h-100">
                  <p class="mb-1 pt-2 text-bold">گروه صادرات یونا</p>
                  <h5 class="font-weight-bolder">Youna Export Group</h5>
                  <p class="mb-5">
                    گروه صادرات یونا با هدف اشتغال زایی و افزایش بهره وری از پتانسیل های نجف آباد شروع به کار کرده است
                  </p>
                  <a
                    class="text-dark font-weight-bold ps-1 mb-0 icon-move-left mt-auto"
                    href="javascript:;"
                  >
                    بیشتر بدانید
                    <i
                      class="fas fa-arrow-left text-sm ms-1"
                      aria-hidden="true"
                    ></i>
                  </a>
                </div>
              </div>
              <div class="col-lg-4 me-auto ms-0 text-center">
                <div
                  class="bg-gradient-success border-radius-lg min-height-200"
                >
                  <img
                    src="../assets/img/shapes/waves-white.svg"
                    class="position-absolute h-100 top-0 d-md-block d-none"
                    alt="waves"
                  />
                  <div class="position-relative pt-5 pb-4">
                    <img
                      class="max-width-500 w-100 position-relative z-index-2"
                      src="../assets/img/illustrations/rocket-white.png"
                    />
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-lg-5">
        <div class="card h-100 p-3">
          <div
            class="overflow-hidden position-relative border-radius-lg bg-cover h-100 new-one">
            <span class="mask bg-gradient-dark"></span>
            <div class="card-body position-relative z-index-1 p-3 h-100">
              <div class="d-flex flex-column h-100">
                <h5 class="text-white font-weight-bolder mb-4 pt-2">
                  به سوی آینده ای بهتر
                </h5>
                <p class="text-white mb-5">
                  نجف آباد شهری که دارای پتانسیل های فراوانی برای افزایش درآمد و صادرات است
                </p>
                <a
                  class="text-white font-weight-bold ps-1 mb-0 icon-move-left mt-auto"
                  href="javascript:;"
                >
                  بیشتر بدانید
                  <i
                    class="fas fa-arrow-left text-sm ms-1"
                    aria-hidden="true"
                  ></i>
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="mt-4 row">
      <div class="col-lg-5 mb-lg-0 mb-4">
        <div class="card">
          <div class="card-body p-3 mt-2">
            <reports-bar-chart
              id="chart-bar"
              title="آمار جامع"
              description="(<strong>+23%</strong>)  از سال 1401"
              :chart="{
                labels: [
                  'Apr',
                  'May',
                  'Jun',
                  'Jul',
                  'Aug',
                  'Sep',
                  'Oct',
                  'Nov',
                  'Dec',
                ],
                datasets: {
                  label: 'صادرات',
                  data: [900, 3000, 1500, 5000, 7000, 5500, 6500, 5100],
                },
              }"
              :items="[
                {
                  icon: {
                    color: 'primary',
                    component: faUsers,
                  },
                  label: 'کاربران فعال',
                  progress: { content: '37K', percentage: 60 },
                },
                {
                  icon: { color: 'info', component: faHandPointer },
                  label: 'مبادلات ارزی',
                  progress: { content: '2m $', percentage: 90 },
                },
                {
                  icon: { color: 'warning', component: faCreditCard },
                  label: 'محصولات موجود',
                  progress: { content: '40', percentage: 30 },
                },
                {
                  icon: { color: 'danger', component: faScrewdriverWrench },
                  label: 'اشتغال',
                  progress: { content: '513', percentage: 70 },
                },
              ]"
            >
            </reports-bar-chart>
          </div>
        </div>
      </div>
      <div class="col-lg-7">
        <gradient-line-chart
          id="chart-line"
          title="آمار ورود و خروج کالا (برحسب تن)"
          description="<i class='fa fa-arrow-up text-success'></i>
      <span class='font-weight-bold'>4% افزایش</span> در مجموع "
          :chart="{
            labels: [
              'Apr',
              'May',
              'Jun',
              'Jul',
              'Aug',
              'Sep',
              'Oct',
              'Nov',
              'Dec',
            ],
            datasets: [
              {
                label: 'ورود کالا',
                data: [500, 400, 3000, 2200, 5000, 2500, 4000, 2300, 5700],
              },
              {
                label: 'خروج کالا',
                data: [300, 250, 2600, 2000, 4500, 3000, 3400, 3000, 4100],
              },
            ],
          }"
        />
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
    TimelineList
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

<style>
.new-one{
  background-image: url('https://demos.creative-tim.com/soft-ui-dashboard/assets/img/ivancik.jpg')
}
</style>