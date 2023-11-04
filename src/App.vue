<template>
  <TheHeader title="Remember Me"/>
  <StoredResources :storedResources="storedResources"/>
</template>

<script>
import StoredResources from "./components/Resources/StoredResources";
import TheHeader from "./components/layouts/TheHeader.vue";
export default {
  name: "App",
  data: () => ({
    storedResources: [
      {
        id: "official-guide",
        title: "Official Guide",
        description: "This is official guide for vuejs",
        link: "https://www.vuejs.org/",
      },
      {
        id: "google",
        title: "Google",
        description: "Just google",
        link: "https://www.google.com/",
      },
    ],
  }),
  components: {
    StoredResources,
    TheHeader
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

</style>
