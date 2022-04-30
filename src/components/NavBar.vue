<template>
  <header>
    <div class="logo">
      <img src="../assets/portfolio_logo.svg" />
      <span class="logo-title"> {{ title }} </span>
    </div>
    <nav>
      <ul class="nav">
        <li>
          <a href="#projects"> {{ navLinks.FirstLink }} </a>
        </li>
        <li>
          <a href="#technologies"> {{ navLinks.SecondLink }} </a>
        </li>
        <li>
          <a href="#aboutMe"> {{ navLinks.ThirdLink }} </a>
        </li>
      </ul>
    </nav>
    <div class="social">
      <ul>
        <li>
          <a
            href="https://github.com/MOUAAD-NASSIH?tab=repositories"
            target="_blank"
            ><img src="../assets/github-icon.svg"
          /></a>
        </li>
        <li>
          <a
            href="https://www.linkedin.com/in/mouaad-nassih-856764230/"
            target="_blank"
            ><img src="../assets/Linkedin-icon.svg"
          /></a>
        </li>
        <li>
          <a href="https://www.figma.com/" target="_blank"
            ><img src="../assets/Figma-icon.svg"
          /></a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      title: "MOU</>D",
      navLinks: {
        FirstLink: "Projects",
        SecondLink: "Technologies",
        ThirdLink: "About Me",
      },
    };
  },
};
</script>

<style scoped>
li {
  list-style: none;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 5.625rem;
  background: transparent;
  padding: 10px 30px;
  margin-bottom: 40px;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-right: 40px;
}

.nav li a {
  display: inline-block;
  color: #fff;
  text-decoration: none;
  font-size: 1rem;
  line-height: 1.25rem;
  padding: 0 40px;
  margin: 20px 0;
  font-weight: 500;
  letter-spacing: 0.8px;
}

.social ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.social ul li a {
  display: inline-block;
  text-decoration: none;
  line-height: 1.25rem;
  padding: 0 15px;
  margin: 20px 0;
}

.logo {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo img,
.logo-title {
  cursor: pointer;
}

.logo-title {
  display: inline-block;
  margin-left: 20px;
  color: #fff;
  font-size: 1.25rem;
  font-weight: 500;
  text-transform: uppercase;
}

/* Mobile */
@media (max-width: 1000px) {
  header {
    display: block;
    /* overflow: hidden; */
  }

  .logo {
    display: block;
    text-align: center;
  }

  .nav {
    display: none;
  }

  .social {
    display: none;
  }

  .logo img {
    width: 4rem;
  }

  .logo-title {
    display: none;
  }
}

/* small screen */
@media (min-width: 768px) {
}

/* medium screen */
@media (min-width: 992px) {
}

/* large screen */
@media (min-width: 1200px) {
}

/* x-large Screen */
@media (min-height: 1700px) {
}
</style>
