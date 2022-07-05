<template>
  <div class="container p-3">
    <div class="d-flex">
        <div class="logo">
            <img :src="logoImg" alt="">
        </div>
        <div class="header-nav ms-auto d-flex gap-5 align-items-baseline">
            <div class="pages-nav">
                <ul class="d-flex list-unstyled gap-4">
                    <li v-for="(page, i) in pagesList" :key="i"><a href="#">{{ page }}</a></li>
                </ul>
            </div>
            <div class="nav-icons d-flex gap-4">
                <a href="#"><i class="fa-solid fa-magnifying-glass"></i></a>
                <div class="position-relative cart">
                    <div class="position-absolute cart-counter">0</div>
                    <a href="#"><i class="fa-solid fa-cart-shopping position-relative"></i></a>
                </div>
            </div>
            <button class="btn btn-primary">Get Started</button>
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
@import "../assets/scss/variables";
.logo {
    img{
        width: 40px;
    }
}

.cart {
    .cart-counter {
        font-size: 12px;
        background-color: $primary;
        border-radius: 50%;
        color: white;
        width: 20px;
        height: 20px;
        transform: translate(50%, -35%);
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .fa-cart-shopping {
        z-index: 1;
    }
}

.header-nav {
    button {
        padding: .5rem 1rem;
    }
}
</style>