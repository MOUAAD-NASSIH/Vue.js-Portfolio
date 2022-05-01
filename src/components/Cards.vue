<template>
  <figure class="card">
    <div class="card-content">
      <img class="card-img" :src="imgCard" />
      <h1 class="card-title">{{ cardTitle }}</h1>
      <p class="card-desc">{{ cardDescription }}</p>
      <button class="card-btn">
        <a :href="liveReview" target="_blank">{{ liveBtn }}</a>
      </button>
      <button class="card-btn">
        <a :href="codeSource" target="_blank">
          {{ codeBtn }}
        </a>
      </button>
    </div>
  </figure>
</template>

<script>
export default {
  data() {
    return {
      liveBtn: "Live",
      codeBtn: "Code",
    };
  },
  props: [
    "cardTitle",
    "cardDescription",
    "imgCard",
    "codeSource",
    "liveReview",
  ],
};
</script>

<style scoped>
.card {
  background-color: transparent;
  border: 5px solid;
  border-image: linear-gradient(#ff512f, #dd2476, #1c64ff) 1;
  animation: rotate 2.5s ease-in infinite;
  margin-bottom: 40px;
}

.card-content {
  max-width: 300px;
  padding: 20px;
  text-align: center;
}

.card-img {
  width: 250px;
  height: 200px;
  margin-bottom: 15px;
  border-radius: 5px;
}

.card-title {
  color: #fff;
  font-size: 25px;
  font-weight: 500;
  text-align: center;
  margin-bottom: 15px;
}

.card-desc {
  color: #fff;
  font-size: 14px;
  font-weight: 200;
  margin-bottom: 15px;
}

.card-btn {
  padding: 5px 20px;
  border: none;
  border-radius: 20px;
  background: linear-gradient(0.25turn, #13adc7, #6978d1, #945dd6);
  margin: 5px 10px;
  cursor: pointer;
}

.card-btn a {
  color: #0f1624;
  text-decoration: none;
  font-weight: 500;
}

@keyframes rotate {
  50% {
    border-image: linear-gradient(360deg, #ff512f, #dd2476, #1c64ff) 1;
  }
}
</style>
