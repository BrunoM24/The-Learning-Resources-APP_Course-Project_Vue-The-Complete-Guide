<template>
  <ul>
    <learning-resource
      v-for="resource in resources"
      :key="resource.id"
      :title="resource.title"
      :description="resource.description"
      :link="resource.link"
    ></learning-resource>
  </ul>
</template>

<script>
import LearningResource from "./LearningResource.vue";
export default {
  name: "StoredResources",
  components: { LearningResource },
  props: {
    resources: [],
  },
};
</script>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  max-width: 40rem;
}
</style>
