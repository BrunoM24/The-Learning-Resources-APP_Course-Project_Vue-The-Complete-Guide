<template>
  <li>
    <div>
      <header>
        <h3>{{ title }}</h3>
        <button>Delete</button>
      </header>
    </div>
    <p>{{ description }}</p>
    <nav>
      <a :href="link" target="_blank">View Resource</a>
    </nav>
  </li>
</template>

<script>
export default {
  name: "LearningResource",
  props: {
    title: String,
    description: String,
    link: String,
  },
};
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

a {
  text-decoration: none;
  color: blueviolet;
}
</style>
