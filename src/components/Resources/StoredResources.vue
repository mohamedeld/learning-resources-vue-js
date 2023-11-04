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
import ResourceItem from "./ResourceItem.vue";
export default{
  components:{ResourceItem},
  props:['storedResources']
}
</script>

<style scoped>
  ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>