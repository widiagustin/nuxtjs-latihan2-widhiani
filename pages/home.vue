<template>
  <div class="items-center justify-center text-center pt-10">
    <h1 class="text-green-600 font-mono text-4xl">Welcome to this page!</h1>
    <p>for the contents</p>
  </div>
</template>
<script>
export default {
  name: "home",
  async asyncData() {
    const api = "https://jsonplaceholder.typicode.com/posts";
    const post = await axios.get(api).then((response) => {
      return response.data;
    });
    return {
      posts,
    };
  },
};
</script>
