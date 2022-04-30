<template>
  <figure class="card">
    <div class="card-content">
      <img class="card-img" src="../assets/logo.png" />
      <h1 class="card-title">{{ cardTitle }}</h1>
      <p class="card-desc">{{ cardDescription }}</p>
      <button class="card-btn">{{ liveBtn }}</button>
      <button class="card-btn">{{ codeBtn }}</button>
    </div>
  </figure>
</template>

<script>
export default {
  data() {
    return {
      cardTitle: "Project # ",
      cardDescription:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt,reprehenderit?",
      liveBtn: "Live",
      codeBtn: "Code",
    };
  },
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

@keyframes rotate {
  50% {
    border-image: linear-gradient(360deg, #ff512f, #dd2476, #1c64ff) 1;
  }
}
</style>
