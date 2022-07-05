<template>
    <div class="position-relative">
        <div class="bg-img position-absolute">
            <img src="/img/14.png" alt="">
        </div>
        <div class="container py-5 position-relative">
            <div class="row">
                <div class="col col-6 flex-grow-1">
                    <h2 class="pb-3">Popular feautures that your business needs</h2>
                    <span class="d-inline-block text-grey pb-5">
                        Faff about only a quid blower I don't want no agro bleeding chimney<br>
                        pot burke tosser cras nice one boot fanny.!
                    </span>
                </div>
                <div class="col align-self-center">
                    <button class="btn btn-primary py-3 px-4">Explore More Feature</button>
                </div>
            </div>

            <div class="row row-cols-4 g-3 gap-3">
                <div class="col shadow" v-for="feature in featuresList" :key="feature.title">
                    <h5>{{ feature.title }}</h5>
                    <img :src="feature.src" :alt="feature.title + ' logo'">
                </div>
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

<style lang="scss" scoped>
@import "../assets/scss/variables";

.container {
    z-index: 1;
}
.bg-img {
    top: 0;
    left: 0;
    transform: translate(-80%, -10%);

    img {
        width: 100%;
    }
}

.shadow {
    box-shadow: 0 0 10px $border-grey;
    width: calc(100% / 4 - 1rem);
}
</style>