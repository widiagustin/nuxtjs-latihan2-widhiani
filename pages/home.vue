<template>
  <div class="items-center justify-center text-center pt-10">
    <h1 class="text-green-600 font-mono text-4xl">Welcome to this page!</h1>
    <p>for the contents</p>
    <nuxt-link
      v-for="post in posts"
      :key="post.id"
      class="list-data"
      :to="'/post/' + post.id"
    >
      {{ post.title }}
    </nuxt-link>
  </div>
</template>
<script>
import axios from "axios";

export default {
  name: "home",
  async asyncData() {
    const { data } = await axios.get(
      "https://jsonplaceholder.typicode.com/posts"
    );
    return { posts: data };
  },
};
</script>
