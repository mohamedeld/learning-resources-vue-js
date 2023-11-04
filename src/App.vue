<template>
  <ul>
    <ResourceItem
      v-for="res in storedResources"
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    />
  </ul>
</template>

<script>
import ResourceItem from "./components/Resources/ResourceItem.vue";

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
    ResourceItem,
  },
};
</script>

<style>
#app {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
