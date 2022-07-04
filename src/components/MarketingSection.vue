<template>
  <div class="container py-5">
    <div class="row">
        <div class="col col-4" v-for="i in 3" :key="i">
            <div class="my-card">
                <div class="card-header d-flex">
                    <img src="/img/24.png" alt="">
                    <div class="text">
                        <h4>Online Marketing</h4>
                        <span>It is a long established fact that a reader will be distracted.</span>
                    </div>
                </div>
                <ul>
                    <li v-for="(element, i) in marketingList" :key="i">
                        <i class="fa-solid fa-check"></i>
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

<style>

</style>