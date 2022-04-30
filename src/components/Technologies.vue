<template>
  <div class="technologies" id="technologies">
    <h1 class="category">{{ categoryTitle }}</h1>
    <div>
      <h2 class="heading">{{ mySkills }}</h2>
    </div>
    <div class="skills-container">
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/Html5-icon.svg" />
        <h3>{{ html }}</h3>
      </div>
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/Css3-icon.svg" />
        <h3>{{ css }}</h3>
      </div>
      <div class="skills-box">
        <img
          class="skills-icon"
          src="../assets/skillsIcons/JavaScript-icon.svg"
        />
        <h3>{{ js }}</h3>
      </div>
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/Git-Icon.svg" />
        <h3>{{ git }}</h3>
      </div>
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/vuejs-icon.svg" />
        <h3>{{ vue }}</h3>
      </div>
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/Scss-icon.svg" />
        <h3>{{ scss }}</h3>
      </div>
      <div class="skills-box">
        <img
          class="skills-icon"
          src="../assets/skillsIcons/figmaSkill-icon.svg"
        />
        <h3>{{ figma }}</h3>
      </div>
      <div class="skills-box">
        <img
          class="skills-icon"
          src="../assets/skillsIcons/bootstrap-icon.svg"
        />
        <h3>{{ b5 }}</h3>
      </div>
    </div>
    <div>
      <h2 class="heading">{{ learning }}</h2>
    </div>
    <div class="skills-container">
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/NodeJs-icon.svg" />
        <h3>{{ node }}</h3>
      </div>
      <div class="skills-box">
        <img class="skills-icon" src="../assets/skillsIcons/mongodb-icon.svg" />
        <h3>{{ mongodb }}</h3>
      </div>
      <div class="skills-box">
        <img
          class="skills-icon"
          src="../assets/skillsIcons/expressjs-icon.svg"
        />
        <h3>{{ express }}</h3>
      </div>
      <div class="skills-box">
        <img
          class="skills-icon"
          src="../assets/skillsIcons/TypeScript-icon.svg"
        />
        <h3>{{ ts }}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      categoryTitle: "Technologies",
      mySkills: "Using Now :",
      learning: "Learning :",
      html: "Html5",
      css: "Css3",
      js: "JavaScript",
      git: "Git",
      vue: "Vue.js",
      scss: "Sass",
      figma: "Figma",
      b5: "Bootstrap",
      node: "Node.js",
      mongodb: "MongoDb",
      express: "Express.js",
      ts: "TypeScript",
    };
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

.technologies {
  margin: 50px 0 180px;
}

.category {
  color: #fff;
  font-size: 40px;
  font-weight: 500;
  text-transform: uppercase;
  padding-bottom: 50px;
}

div .heading {
  font-family: "Montserrat", sans-serif;
  font-weight: 400;
  color: #fff;
  line-height: 80px;
  letter-spacing: 1.4px;
  padding: 10px 20px;
}

.skills-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(17rem, 1fr));
  margin-bottom: 2rem;
  gap: 2rem;
}

.skills-box {
  text-align: center;
}

.skills-icon {
  height: 100px;
  cursor: pointer;
}

.skills-box h3 {
  font-family: "Montserrat", sans-serif;
  font-weight: 400;
  color: #fff;
  line-height: 50px;
  letter-spacing: 1.4px;
  text-transform: uppercase;
}
</style>
