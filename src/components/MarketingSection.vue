<template>
  <div class="container py-5">
    <div class="row">
        <div class="col col-4" v-for="i in 3" :key="i">
            <div class="my-card">
                <div class="card-header d-flex pb-4 gap-3">
                    <img src="/img/24.png" alt="">
                    <div class="text">
                        <h4>Online Marketing</h4>
                        <span class="text-grey">It is a long established fact that a reader will be distracted.</span>
                    </div>
                </div>
                <ul class="list-unstyled">
                    <li class="pb-3" v-for="(element, i) in marketingList" :key="i">
                        <i class="fa-solid fa-check text-primary me-3"></i>
                        {{ element }}
                    </li>
                </ul>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
data() {
    return {
        marketingList: [
            "SEO",
            "SEM",
            "Website strategy",
            "Social management",
        ]
    }
}
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";
.card-header {
    img {
        width: 80px;
        height: 80px;
    }
}

.my-card {
    ul {
        padding-left: calc(80px + 1rem);
    }
}
</style>