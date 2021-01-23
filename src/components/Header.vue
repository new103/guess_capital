<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<script>
export default {
  data() {
    return {
      title: "Guess Capital",
    };
  },
};
</script>

<style scoped>
header {
  background: #0d6efd;
  padding: 2rem;
  text-align: center;
  color: #fff;
  letter-spacing: 0.25rem;
}
</style>