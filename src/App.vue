<template>
  <stored-resources :resources="storedResources"></stored-resources>
</template>

<script>
import StoredResources from "./components/learning-resources/StoredResources.vue";

export default {
  components: { StoredResources },
  data() {
    return {
      storedResources: [
        {
          id: "official-guide",
          title: "Official Guide",
          description: "The Official VueJS Documentation",
          link: "https://vuejs.org",
        },
        {
          id: "google-guide",
          title: "Google Guide",
          description: "Learn to google...",
          link: "https://google.com",
        },
      ],
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;
}
</style>
