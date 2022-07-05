<template>
    <div class="border-top border-gray">
        <div class="container py-5">
            <div class="row gap-5">
                <div class="col col-3 me-5">
                    <!-- logo + testo -->
                    <img class="pb-2" :src="footerLogo" alt="">

                    <div class="footer-text text-grey pb-5">It is a long established fact that a reader will be
                        distracted by the readable content.</div>
                    <span class="text-grey">Copyright @ 2018 <span class="text-primary">Sofbox</span></span>
                </div>
                <div class="col col-2">
                    <!-- Menù + ul -->
                    <h5 class="pb-4">Menu</h5>
                    <ul>
                        <li v-for="link in linksList" :key="link"><a class="text-grey d-inline-block pb-3" href="#">{{
                                link
                        }}</a></li>
                    </ul>
                </div>
                <div class="col col-2">
                    <!-- About us + ul -->
                    <h5 class="pb-4">About Us</h5>
                    <ul>
                        <li v-for="link in aboutUsLinks" :key="link"><a class="text-grey d-inline-block pb-3"
                                href="#">{{ link }}</a></li>
                    </ul>
                </div>
                <div class="col col-2">
                    <!-- Quick links + ul -->
                    <h5 class="pb-4">Quick Links</h5>
                    <ul>
                        <li v-for="link in linksList" :key="link"><a class="text-grey d-inline-block pb-3" href="#">{{
                                link
                        }}</a></li>
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