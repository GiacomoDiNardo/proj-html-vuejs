<template>
  <div class="container py-5">
    <div class="row">
        <div class="col col-6">
            <h1>The biggest platform for your growth.</h1>
            <span>There are many variations of passages of Lorem Ipsum avaiable, but the majority have suffered alteration in some form</span>
            <button class="btn btn-primary">Read more</button>
        </div>
        <div class="col col-6">
            <img :src="jumboImg" alt="jumbotron image">
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

<style>

</style>