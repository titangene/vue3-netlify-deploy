<template>
  <div class="home">
    <img alt="Vue logo" src="@/assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App (main lock + 2)" />
    <p>{{ apiBaseURL }}</p>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  },
  setup() {
    const apiBaseURL = process.env.VUE_APP_API_BASE_URL;
    return {
      apiBaseURL
    };
  }
};
</script>
