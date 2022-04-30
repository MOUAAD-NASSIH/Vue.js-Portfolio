<template>
  <div class="footer">
    <h3>Copyrights @ <span class="name">Mouaad Nassih</span></h3>
    <ul>
      <li>
        <a
          href="https://github.com/MOUAAD-NASSIH?tab=repositories"
          target="_blank"
          ><img src="../assets/github-icon.svg" alt=""
        /></a>
      </li>
      <li>
        <a
          href="https://www.linkedin.com/in/mouaad-nassih-856764230/"
          target="_blank"
          ><img src="../assets/Linkedin-icon.svg" alt=""
        /></a>
      </li>
      <li>
        <a href="https://www.figma.com/" target="_blank"
          ><img src="../assets/Figma-icon.svg" alt=""
        /></a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 80px;
  margin-top: 100px;
}

.footer ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer ul li {
  list-style: none;
}

.footer ul li a {
  padding: 0 20px;
}

.footer h3 {
  color: #fff;
}

.footer span {
  color: #3b62b0;
}
</style>
