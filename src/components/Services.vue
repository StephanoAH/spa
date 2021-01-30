<template>
  <section id="services" class="services">
    <div class="services__container">
      <h2>Services</h2>
      <div class="services__grid">
        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-1.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <h3>Service 1</h3>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
            optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
            quis cumque odio perferendis in facere aliquid praesentium placeat
            maxime ab.
          </p>
        </div>

        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-2.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <h3>Service 2</h3>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
            optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
            quis cumque odio perferendis in facere aliquid praesentium placeat
            maxime ab.
          </p>
        </div>

        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-3.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <h3>Service 3</h3>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
            optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
            quis cumque odio perferendis in facere aliquid praesentium placeat
            maxime ab.
          </p>
        </div>

        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-4.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <h3>Service 4</h3>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
            optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
            quis cumque odio perferendis in facere aliquid praesentium placeat
            maxime ab.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style lang="scss" scoped>
.services {
  background-color: #eee;

  .services__container {
    padding: 1em 0;

    h2 {
      text-align: center;
      text-transform: uppercase;
      color: #313;
      font-size: 2rem;
    }

    .services__grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 1em;
      padding: 0.5em;

      .service {
        p {
          text-align: justify;
        }

        .service__image {
          max-width: 100%;
        }
      }
    }
  }
}
</style>
