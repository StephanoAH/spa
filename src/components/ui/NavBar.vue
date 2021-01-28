<template>
  <header>
    <div class="container">
      <h2>PORTFOLIO</h2>
      <nav>
        <a href="#">Home</a>
        <a href="">Services</a>
        <a href="">Projects</a>
        <a href="">Contact</a>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style lang="scss" scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 2;
  color: #fff;
  background-color: #12002f;

  .container {
    display: flex;
    align-items: baseline;
    justify-content: space-between;

    max-width: 1600px;
    margin: 0 auto;
    padding-left: 2rem;
    padding-right: 2rem;
  }

  h2 {
    color: inherit;
    font-weight: 900;
    font-size: 1.7rem;
  }

  nav {
    display: grid;
    gap: 1rem;
    grid-template-columns: repeat(4, auto);

    a {
      color: inherit;
      font-size: 1.3rem;
      text-decoration: none;
    }
  }
}
</style>
