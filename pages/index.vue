<template>
  <div>
    <home />
  </div>
</template>

<script>
import axios from "axios";
import AppLogo from "~/components/AppLogo.vue";
import Home from "./home.vue";

export default {
  components: {
    AppLogo,
    home: Home,
  },
};
</script>

<style>
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
</style>
