<template>
  <main>
    <section class="banner">
      <div class="banner__container">
        <h1>
          Websites you're <br class="hide--mobile" />
          <span>not afraid</span> to share
        </h1>
        <h2>Websites solutions for all your needs</h2>
        <a href="#" class="banner__buton">Find out more</a>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style lang="scss" scoped>
$pink: #ff9fdb;

main {
  section.banner {
    position: relative;
    min-height: 100vh;
    display: flex;
    align-items: center;
    background-image: url(../assets/images/header1.jpg);
    background-position: center;
    background-size: cover;
    margin: -0.5em;

    &:after {
      content: "";
      display: block;
      position: absolute;
      top: 0;
      right: 0;
      bottom: 0;
      left: 0;
      z-index: 0;
      background-color: #12002f;
      opacity: 0.8;
    }

    .banner__container {
      padding-left: 2em;
      position: relative;
      z-index: 1;
      color: #fff;

      h1 {
        font-size: 3.5rem;
        margin-bottom: 0;
        span {
          color: $pink;
        }
      }

      h2 {
        font-size: 2rem;
        font-weight: 400;
      }

      .banner__buton {
        display: inline-block;
        color: #fff;
        background-color: $pink;
        padding: 0.8em 1em;
        border-radius: 0.5em;
        text-decoration: none;
        text-transform: uppercase;
        font-weight: 700;
      }
    }
  }
}
</style>
