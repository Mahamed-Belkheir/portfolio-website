<template>
  <nav class="navbar">
      <ul class="nav-items">
          <li>About</li>
          <li>Experience</li>
          <li>Projects</li>
          <!-- <li>Blog</li> -->
          <li>Contact</li>
      </ul>
  </nav>
</template>

<script>
export default {

}
</script>

<style scoped>
.navbar {
    width: 100%;
    display: flex;
    justify-content: flex-end;
    overflow: hidden;
    z-index: 100;
    position: fixed;
}

.nav-items {
    display: flex;
    width: 30%;
    justify-content: space-around;
    list-style: none;
    margin-right: 10%;
    font-size: 24px;
}

li {
    margin-right: 10px;
}

</style>