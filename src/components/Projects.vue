<template>
  <div class="projects" id="projects">
    <h1 class="category">{{ categoryTitle }}</h1>
    <div class="cards-container">
      <Cards
        class="card"
        cardTitle="CocaCola Clone"
        cardDescription="Building a similar website to cocacola.com"
        :imgCard="imgCard1"
        codeSource="https://github.com/MOUAAD-NASSIH/CocaCola-Clone"
        liveReview="https://cocacola-clone.netlify.app//"
      />
      <Cards
        class="card"
        cardTitle="StarBucks Clone"
        cardDescription="Building a similar website to starbucks.com"
        :imgCard="imgCard2"
        codeSource="https://github.com/MOUAAD-NASSIH/Starbucks-Clone"
        liveReview="https://starbucks-clone-website.netlify.app//"
      />
      <Cards
        class="card"
        cardTitle="Pepsi Clone"
        cardDescription="Building a similar website to pepsi.com"
        :imgCard="imgCard3"
        codeSource="https://github.com/MOUAAD-NASSIH/Pepsi-Clone"
        liveReview="https://pepsi-clone.netlify.app//"
      />
    </div>
    <div class="more-projects">
      <button>
        <a href="https://github.com/MOUAAD-NASSIH?tab=repositories">{{
          btn
        }}</a>
      </button>
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
      imgCard1: require("../assets/starbucks.jpg"),
      imgCard2: require("../assets/starbucks.jpg"),
      imgCard3: require("../assets/starbucks.jpg"),
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

.more-projects button a {
  color: #0f1624;
  text-decoration: none;
  font-weight: 500;
}
</style>
