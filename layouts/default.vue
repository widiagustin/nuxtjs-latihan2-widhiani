<template>
  <div>
    <nav-bar />
    <nuxt />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
export default {
  components: {
    "nav-bar": Navbar,
  },
};
</script>

