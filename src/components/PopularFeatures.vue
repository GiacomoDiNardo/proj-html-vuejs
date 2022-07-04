<template>
  <div class="container py-5">
    <div class="row">
      <div class="col col-6 flex-grow-1">
        <h2>Get tips tricks on how to skyrocket you sales.</h2>
        <span>
          Faff about only a quid blower I don't want no agro bleeding chimney<br>
          pot burke tosser cras nice one boot fanny.!
        </span>
      </div>
      <div class="col">
        <button class="btn btn-primary">Explore More Feature</button>
      </div>
    </div>

    <div class="row g-3">
        <div class="col col-3" v-for="feature in featuresList" :key="feature.title">
            <h5>{{ feature.title }}</h5>
            <img :src="feature.src" :alt="feature.title + ' logo'">
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            featuresList: [
                {
                    title: "Customized Invoices",
                    src: ""
                },
                {
                    title: "Stock Management",
                    src: ""
                },
                {
                    title: "Receivable & Payable",
                    src: ""
                },
                {
                    title: "Manage Buying",
                    src: ""
                },
                {
                    title: "Powerful & Secure",
                    src: ""
                },
                {
                    title: "Fastest Return Filing",
                    src: ""
                },
                {
                    title: "Montly Detailed",
                    src: ""
                },
                {
                    title: "Product Management",
                    src: ""
                },
            ]
        }
    }
};
</script>

<style>
</style>