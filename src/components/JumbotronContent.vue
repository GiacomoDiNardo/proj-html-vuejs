<template>
    <div class="jumbo-bg mb-5">
        <div class="my-container p-5">
            <div class="row">
                <div class="col col-6">
                    <h1 class="pb-3">The biggest platform for your growth.</h1>
                    <span class="pb-5 d-block text-grey">There are many variations of passages of Lorem Ipsum avaiable, but the majority have suffered
                        alteration in some form</span>
                    <button class="btn btn-primary">Read more</button>
                </div>
                <div class="col col-6">
                    <img class="jumbo-img" :src="jumboImg" alt="jumbotron image">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            jumboImg: "/img/27-1.png"
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

.jumbo-bg {
    background-color: $bg-primary;
    width: 1100px;
    margin: auto;
    position: relative;
    padding-top: 80px;

    .jumbo-img {
        width: 50%;
        position: absolute;
        top: 100px;
        right: 0;
    }
}
</style>