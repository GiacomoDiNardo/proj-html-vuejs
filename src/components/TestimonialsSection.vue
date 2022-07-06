<template>
  <div class="container py-5">
    <div class="text-center">
        <h2>Our Testimonials</h2>
        <span class="text-grey pb-5 d-inline-block">If you are planning on developing a product landing app or website,<br> take a look at this beautiful-crafted</span>
    </div>
    
    <div class="row justify-content-center">
        <div class="col col-6">
            <div class="card p-3 text-center">
                <img class="m-auto my-4" src="/img/26.jpeg" alt="">
                <h5>Julia Aann</h5>
                <span class="text-grey pb-4">- COO Sofbox</span>
                <p class="text-grey text-start">
                    At vero eos et accusamus et iusto odio dignissimos
                    ducimus qui blanditiis praesentium vero eos et consectetur
                    accus adip adip.
                </p>
            </div>
        </div>
        <div class="col col-6">
            <div class="card p-3 text-center">
                <img class="m-auto my-4" src="/img/27.jpeg" alt="">
                <h5>Mac Znder</h5>
                <span class="text-grey pb-4">- Manager Sofbox</span>
                <p class="text-grey text-start">
                    At vero eos et accusamus et iusto odio dignissimos
                    ducimus qui blanditiis praesentium vero eos et consectetur
                    accus adip adip.
                </p>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

.card {
    
    img {
        width: 70px;
        border-radius: 50%;
        border: 1px solid white;
        box-shadow:  0 0 10px $border-grey;
    }

    h5, span {
        display: inline-block;
    }
}
</style>