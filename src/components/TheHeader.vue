<template>
  <div class="container p-3">
    <div class="d-flex">
        <div class="logo">
            <img :src="logoImg" alt="">
        </div>
        <div class="header-nav ms-auto d-flex gap-5 align-items-center">
            <div class="pages-nav">
                <ul class="d-flex list-unstyled gap-4 align-items-baseline">
                    <li v-for="(page, i) in pagesList" :key="i"><a href="#">{{ page }}</a></li>
                </ul>
            </div>
            <div class="nav-icons d-flex gap-3">
                <i class="fa-solid fa-magnifying-glass"></i>
                <i class="fa-solid fa-cart-shopping"></i>
            </div>
            <button class="btn btn-primary p-3">Get Started</button>
        </div>
    </div>

  </div>
</template>

<script>
export default {
    data() {
        return {
            logoImg: "/img/logo-2.png",
            pagesList: [
                "Home",
                "About us",
                "Feauture",
                "Testimonials",
                "Contact us",

            ]
        }
    }

}
</script>

<style lang="scss" scoped>
.logo {
    img{
        width: 40px;
    }
}

.pages-nav {
    li {
        a {
            color: black;
            text-decoration: none;
        }
    }
}
</style>