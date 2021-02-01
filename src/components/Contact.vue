<template>
  <section id="contact" class="contact">
    <div class="contact__container">
      <h2>Contact</h2>
      <form>
        <div class="contactForm__grid">
          <input
            type="text"
            id="name"
            name="name"
            placeholder="Name"
            class="contactForm__element"
          />
          <input
            type="text"
            id="email"
            name="email"
            placeholder="test@email.com"
            class="contactForm__element"
          />
          <textarea
            name="message"
            id="message"
            placeholder="Tell me your idea..."
            class="contactForm__area"
          ></textarea>
        </div>
        <div class="button--center">
          <input type="submit" value="Send message" class="contact__button" />
        </div>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style lang="scss" scoped>
.contact {
  background-color: #9b75d7;

  .contact__container {
    padding: 1em;

    @media (max-width: 1024px) {
      height: 600px;
    }

    @media (max-width: 768px) {
      height: 850px;
    }

    @media (max-width: 768px) {
      height: 580px;
    }
    h2 {
      text-align: center;
      color: #fff;
      font-size: 2rem;
      text-transform: uppercase;
    }

    form {
      display: block;
      margin: 0 auto;
      max-width: 600px;

      .contactForm__grid {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 1em;

        .contactForm__element {
          appearance: none;
          border: none;
          outline: none;
          background: none;

          display: block;
          background-color: #fff;
          border-radius: 0.5em;

          padding: 1em;
          color: #313;

          &::placeholder {
            color: #aaa;
          }
        }

        .contactForm__area {
          appearance: none;
          border: none;
          outline: none;
          background: none;

          display: block;
          background-color: #fff;
          border-radius: 0.5em;
          height: 150px;

          padding: 1em;
          color: #313;

          &::placeholder {
            color: #aaa;
          }
        }

        .contactForm__area {
          grid-column: 1/-1;
        }
      }

      .button--center {
        text-align: center;

        .contact__button {
          appearance: none;
          border: none;
          outline: none;
          background: none;
          cursor: pointer;

          color: #fff;
          background-color: #ff9fdb;
          padding: 0.8em 1em;
          margin: 1em;
          border-radius: 0.5em;
          text-decoration: none;
          text-transform: uppercase;
          font-weight: 700;

          @media (max-width: 1024px) {
            margin: 2em;
          }

          @media (max-width: 768px) {
            padding: 1em;
          }
        }
      }
    }
  }
}
</style>
