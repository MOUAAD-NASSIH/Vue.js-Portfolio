<template>
  <div class="content">
    <h1>
      {{ heading }} <span> {{ code }} </span>
    </h1>
    <div class="para-wrap">
      <p>{{ paragraph }}</p>
    </div>
    <button>
      <a href="#projects">{{ btn }}</a>
    </button>
    <div class="bg-drawing"><img src="../assets/bg-drawing.svg" /></div>

    <div class="scroll-container">
      <h3>{{ mouseIcon }}</h3>
      <div class="scroll-down">
        <span class="mouse">
          <span class="mouse-wheel"></span>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      heading: "Future Full Stack Developer",
      code: "</>",
      paragraph:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
      btn: "Let’s begin",
      mouseIcon: "scroll down",
    };
  },
};
</script>

<style scoped>
.content {
  width: 100%;
  padding: 50px 100px;
}

.bg-drawing {
  position: absolute;
  top: 0;
  right: 0;
  z-index: -1;
}

.content h1 {
  padding: 10px;
  font-size: 5rem;
  font-weight: 800;
  color: #fff;
  letter-spacing: 1px;
}

.content span {
  font-size: 6.25rem;
  font-weight: 800;
  font-family: "consolas";
  color: #fff;
}

.content .para-wrap {
  padding: 20px 10px;
  color: #fff;
  width: 60%;
  font-size: 1.125rem;
  margin: 20px;
}

.content button {
  padding: 10px 30px;
  color: #fff;
  border: none;
  border-radius: 2.5rem;
  font-size: 1rem;
  font-weight: 500;
  cursor: pointer;
  margin: 10px 0 20px 40px;
  background: linear-gradient(0.25turn, #13adc7, #6978d1, #945dd6);
}

.content button a {
  text-decoration: none;
  color: #fff;
}

.scroll-container {
  padding: 40px 0;
  text-align: center;
}

.scroll-container h3 {
  color: #fff;
  font-family: "consolas";
  font-weight: 100;
  padding: 10px 0;
}

.scroll-down {
  display: flex;
  justify-content: center;
  align-items: center;
}

.mouse {
  width: 1.563rem;
  height: 3.125rem;
  border: 2px solid #fff;
  border-radius: 1.25rem;
  display: flex;
  cursor: pointer;
}

.mouse-wheel {
  display: block;
  width: 0.625rem;
  height: 0.625rem;
  background-color: #fff;
  border-radius: 50%;
  margin: auto;
  animation: move-wheel 1s linear infinite;
}

@media (max-width: 1000px) {
  .content {
    padding: 50px 10px;
    text-align: center;
  }

  .bg-drawing {
    height: calc(100vh - 400px);
    position: absolute;
    top: 0;
    right: 0;
    z-index: -1;
  }

  .content h1 {
    padding: 5px;
    font-size: 3.5rem;
    font-weight: 600;
    color: #fff;
    letter-spacing: 0.8px;
  }

  .content .para-wrap {
    padding: 20px 10px;
    color: #fff;
    width: 100%;
    font-size: 1rem;
    margin: 0px;
  }

  .content button {
    margin: 0;
  }

  .scroll-container {
    display: none;
  }
}

@keyframes move-wheel {
  0% {
    opacity: 0;
    transform: translateY(-1rem);
  }

  100% {
    opacity: 1;
    transform: translateY(1rem);
  }
}
</style>
