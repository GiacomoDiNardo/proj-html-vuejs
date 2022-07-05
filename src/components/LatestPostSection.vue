<template>
  <div class="container py-5">
    <div class="text-center">
        <h2>Latest Posts</h2>
        <span>If you are planning on developing a product landing.</span>
    </div>

    <div class="row">
        <div class="col col-4" v-for="(post, i) in postsList" :key="i">
            <div class="card">
                <img :src="post.src" :alt="post.title + ' img'">
                <h5>{{ post.title }}</h5>
                <span>{{ post.text }}</span>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            postsList: [
                {
                    src: "/img/19.jpg",
                    date: "November 28, 2019",
                    title: "Life Lack Meaning",
                    text: "It is a long established fact that a reader will be distracted by the readable"
                },
                {
                    src: "/img/18.jpg",
                    date: "November 28, 2019",
                    title: "Life Lack Meaning",
                    text: "It is a long established fact that a reader will be distracted by the readable"
                },
                {
                    src: "/img/17.jpg",
                    date: "November 28, 2019",
                    title: "Life Lack Meaning",
                    text: "It is a long established fact that a reader will be distracted by the readable"
                },
            ]
        }
    }
}
</script>

<style>

</style>