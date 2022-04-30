<template>
  <div class="projects" id="projects">
    <h1 class="category">{{ categoryTitle }}</h1>
    <div class="cards-container">
      <Cards class="card" />
      <Cards class="card" />
      <Cards class="card" />
    </div>
    <div class="more-projects">
      <button>{{ btn }}</button>
    </div>
  </div>
</template>

<script>
import Cards from "../components/Cards.vue";
export default {
  components: {
    Cards,
  },
  data() {
    return {
      categoryTitle: "Projects",
      btn: "See More projects",
    };
  },
};
</script>

<style scoped>
.projects {
  margin: 50px 0 190px;
}

.category {
  color: #fff;
  font-size: 40px;
  font-weight: 500;
  text-transform: uppercase;
  padding-bottom: 50px;
}

.cards-container {
  display: flex;
  width: 100%;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
}

.card {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.more-projects {
  text-align: center;
}

.more-projects button {
  border: none;
  border-radius: 40px;
  padding: 15px 50px;
  background: linear-gradient(0.25turn, #13adc7, #6978d1, #945dd6);
  margin-top: 20px;
  cursor: pointer;
}
</style>
