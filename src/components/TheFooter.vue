<template>
  <div class="container">
    <div class="row gap-5">
        <div class="col col-3 me-5">
            <!-- logo + testo -->
            <img :src="footerLogo" alt="">

            <div class="footer-text">It is a long established fact that a reader will be distracted by the readable content.</div>
            <span>Copyright @ 2018 Sofbox</span>
        </div>
        <div class="col col-2">
            <!-- Menù + ul -->
            <h5>Menu</h5>
            <ul>
                <li v-for="link in linksList" :key="link"><a href="#">{{ link }}</a></li>
            </ul>
        </div>
        <div class="col col-2">
            <!-- About us + ul -->
            <h5>About Us</h5>
            <ul>
                <li v-for="link in aboutUsLinks" :key="link"><a href="#">{{ link }}</a></li>
            </ul>
        </div>
        <div class="col col-2">
            <!-- Quick links + ul -->
            <h5>Quick Links</h5>
            <ul>
                <li v-for="link in linksList" :key="link"><a href="#">{{ link }}</a></li>
            </ul>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            footerLogo: "/img/35.png",
            linksList: [
                "About us",
                "Theme",
                "Features",
                "Pricing",
                "Blog",
            ],
            aboutUsLinks: [
                "About Sofbox",
                "Roadmap",
                "How it work",
                "Team",
                "News",
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.col {
    ul {
        list-style: none;
        text-align: start;
        padding-left: 0;
    }
}


</style>