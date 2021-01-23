<template>
  <footer>
    <p>{{ author }}</p>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      author: "Created by Tomasz Waligóra",
    };
  },
};
</script>

<style scoped>
footer {
  background: #0d6efd;
}

p {
  color: #fff;
  text-align: center;
  padding: 1rem;
}
</style>