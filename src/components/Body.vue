<template>
  <main>
    <ul>
      <li v-for="capital of capitals" v-on:click="capital.show = !capital.show">
        <h2>{{ capital.country }}</h2>
        <h3 v-show="capital.show">{{ capital.capital }}</h3>
      </li>
    </ul>
  </main>
</template>

<script>
export default {
  data() {
    return {
      capitals: [
        { country: "Poland", capital: "Warsaw", show: false },
        { country: "The Netherlands", capital: "The Hague", show: false },
        { country: "Germany", capital: "Berlin", show: false },
        { country: "France", capital: "Paris", show: false },
        { country: "Belgium", capital: "Brussels", show: false },
        { country: "Spain", capital: "Madrid", show: false },
      ],
    };
  },
};
</script>

<style scoped>
main {
  /* background: yellow; */
  width: 100%;
  max-width: 75rem;
  margin: 2.5rem auto;
  padding: 0 1.25rem;
}

ul {
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  padding: 0;
}

li {
  flex-grow: 1;
  flex-basis: 18.75rem;
  height: 9rem;
  text-align: center;
  margin: 1rem;
  padding: 2rem;
  background: #9ac2fe;
  border-radius: 10px;
  transition: all 0.5s linear;
}

li:hover {
  background: #81b3fe;
  cursor: pointer;
}

h2 {
  margin-bottom: 2rem;
}
</style>