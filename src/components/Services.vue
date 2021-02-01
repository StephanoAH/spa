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
          <div class="service__content">
            <h3>Service 1</h3>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
              optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
              quis cumque odio perferendis in facere aliquid praesentium placeat
              maxime ab.
            </p>
          </div>
        </div>

        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-2.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <div class="service__content">
            <h3>Service 2</h3>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
              optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
              quis cumque odio perferendis in facere aliquid praesentium placeat
              maxime ab.
            </p>
          </div>
        </div>

        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-3.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <div class="service__content">
            <h3>Service 3</h3>
            <p>
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Veniam
              optio saepe ipsum, atque quibusdam porro officiis maxime! Ad quos,
              quis cumque odio perferendis in facere aliquid praesentium placeat
              maxime ab.
            </p>
          </div>
        </div>

        <div class="service">
          <figure class="service__imageBox">
            <img
              src="../assets/images/service-4.jpg"
              alt=""
              class="service__image"
            />
          </figure>
          <div class="service__content">
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
    </div>
  </section>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style lang="scss" scoped>
$pink: #ff9fdb;
.services {
  background-color: #eee;

  .services__container {
    padding: 2em 0;

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
      padding: 0.5em 3em;

      @media (max-width: 1024px) {
        grid-template-columns: repeat(2, 1fr);
      }

      @media (max-width: 414px) {
        grid-template-columns: repeat(1, 1fr);
      }

      .service {
        background-color: #fff;
        border-radius: 1em;
        overflow: hidden;
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);

        p {
          text-align: justify;
        }

        .service__imageBox {
          display: contents;
          width: 100%;

          .service__image {
            display: block;
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-bottom: 5px solid $pink;
          }
        }

        .service__content {
          padding: 0 0.5em;
        }
      }
    }
  }
}
</style>
