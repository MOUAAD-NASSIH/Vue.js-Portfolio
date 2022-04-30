<template>
  <div class="aboutMe" id="aboutMe">
    <h1 class="category">{{ categoryTitle }}</h1>
    <div class="about-container">
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nam quisquam
        eaque rem ratione quod quos maxime, repudiandae deleniti! Expedita
        temporibus, eaque sapiente est reprehenderit recusandae dolore dolores
        laudantium, eius consequuntur illum tempore! Unde vero iure accusantium
        quos obcaecati, iste laudantium excepturi vel ab iusto nihil molestias
        ipsam architecto, reiciendis quasi eius consequuntur tempora ea velit!
        Sint id veritatis illo magnam quidem nobis voluptas recusandae delectus,
        qui dolores voluptate eaque ipsam totam ipsum iure voluptatem odit
        molestias consequatur vel excepturi corporis. Deleniti sint, labore unde
        delectus ad neque illum, maxime corrupti reprehenderit fuga ut nobis
        sapiente vero impedit esse suscipit repellendus.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      categoryTitle: "About Me",
    };
  },
};
</script>

<style scoped>
.aboutMe {
  margin: 50px 0 180px;
}

.category {
  color: #fff;
  font-size: 40px;
  font-weight: 500;
  text-transform: uppercase;
  padding-bottom: 50px;
}

.about-container {
  width: 100%;
}

.about-container p {
  color: #fff;
  font-weight: 500;
  letter-spacing: 1px;
  padding: 20px 50px;
}
</style>
