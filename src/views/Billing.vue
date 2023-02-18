<template>
  <div class="container-fluid mt-4">
    <div class="row align-items-center">
    </div>
    <div class="row">
      <div class="col-lg-8">
        <div class="row mt-4">
          <div class="col-xl-6">
            <div class="row">
              <div class="col-md-6">
                <default-info-card
                  icon="text-white fas fa-landmark"
                  title="Salary"
                  description="Belong Interactive"
                  value="+$2000"
                />
              </div>
              <div class="col-md-6">
                <default-info-card
                  icon="text-white fab fa-paypal"
                  title="Paypal"
                  description="Freelance Payment"
                  value="$455.00"
                />
              </div>
            </div>
          </div>
          <div class="col-md-12 mb-4">
            <payment-methods-card />
          </div>
        </div>
      </div>
      <div class="">
        <invoice-card />
      </div>
    </div>
    <div class="row mt-4">
      <div class="mt-4">
        <billing-card
          title="مشتریان"
          :bills="[
            {
              name: 'علی محمدی',
              company: 'صادرات',
              email: 'oliver@burrito.com',
              id: 'FRB1235476',
            },
            {
              name: 'رضا اسدی',
              company: 'سنگ',
              email: 'lucas@stone-tech.com',
              id: 'FRB1235476',
            },
            {
              name: 'سعید',
              company: 'کشاورزی',
              email: 'ethan@fiber.com',
              id: 'FRB1235476',
            },
          ]"
        />
      </div>
      <div class="col-md-5 mt-4">
        
      </div>
    </div>
  </div>
</template>

<script>
import setTooltip from "@/assets/js/tooltip.js";
import InvoiceCard from "./components/InvoiceCard.vue";
import BillingCard from "./components/BillingCard.vue";

export default {
  name: "Billing",
  components: {
    InvoiceCard,
    BillingCard
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
