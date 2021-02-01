<template>
  <section id="projects" class="projects">
    <div class="projects__container">
      <h2>Projects</h2>
      <div class="projects__grid">
        <div class="project">
          <figure class="project__imgBox">
            <img
              src="../assets/images/project-img.jpg"
              alt=""
              class="project__img"
            />
          </figure>
          <div class="project__img--overlay">
            <div class="project__content">
              <h3>Project 1</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptates nostrum vitae tempora cum iste possimus corrupti
                ratione totam ipsa? Magni!
              </p>
              <a href="" class="project__button">See more</a>
            </div>
          </div>
        </div>

        <div class="project">
          <figure class="project__imgBox">
            <img
              src="../assets/images/project-img.jpg"
              alt=""
              class="project__img"
            />
          </figure>
          <div class="project__img--overlay">
            <div class="project__content">
              <h3>Project 2</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptates nostrum vitae tempora cum iste possimus corrupti
                ratione totam ipsa? Magni!
              </p>
              <a href="" class="project__button">See more</a>
            </div>
          </div>
        </div>

        <div class="project">
          <figure class="project__imgBox">
            <img
              src="../assets/images/project-img.jpg"
              alt=""
              class="project__img"
            />
          </figure>
          <div class="project__img--overlay">
            <div class="project__content">
              <h3>Project 3</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptates nostrum vitae tempora cum iste possimus corrupti
                ratione totam ipsa? Magni!
              </p>
              <a href="" class="project__button">See more</a>
            </div>
          </div>
        </div>

        <div class="project">
          <figure class="project__imgBox">
            <img
              src="../assets/images/project-img.jpg"
              alt=""
              class="project__img"
            />
          </figure>
          <div class="project__img--overlay">
            <div class="project__content">
              <h3>Project 4</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptates nostrum vitae tempora cum iste possimus corrupti
                ratione totam ipsa? Magni!
              </p>
              <a href="" class="project__button">See more</a>
            </div>
          </div>
        </div>

        <div class="project">
          <figure class="project__imgBox">
            <img
              src="../assets/images/project-img.jpg"
              alt=""
              class="project__img"
            />
          </figure>
          <div class="project__img--overlay">
            <div class="project__content">
              <h3>Project 5</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptates nostrum vitae tempora cum iste possimus corrupti
                ratione totam ipsa? Magni!
              </p>
              <a href="" class="project__button">See more</a>
            </div>
          </div>
        </div>

        <div class="project">
          <figure class="project__imgBox">
            <img
              src="../assets/images/project-img.jpg"
              alt=""
              class="project__img"
            />
          </figure>
          <div class="project__img--overlay">
            <div class="project__content">
              <h3>Project 6</h3>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Voluptates nostrum vitae tempora cum iste possimus corrupti
                ratione totam ipsa? Magni!
              </p>
              <a href="" class="project__button">See more</a>
            </div>
          </div>
        </div>
      </div>
      <div class="project__button__container">
        <a href="" class="projects__button">Show more</a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Projects",
};
</script>

<style lang="scss" scoped>
$pink: #ff9fdb;

.projects {
  background: #fff;
  .projects__container {
    margin: 0 1em;

    h2 {
      text-align: center;
      text-transform: uppercase;
      font-size: 2rem;
    }

    .projects__grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-template-rows: repeat(2, 1fr);
      gap: 1em;

      .project {
        height: 220px;
        position: relative;
        background-color: #fff;
        border-radius: 1em;
        overflow: hidden;
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);

        .project__imgBox {
          display: contents;
          width: 100%;

          .project__img {
            display: block;
            position: relative;
            width: 100%;
            object-fit: cover;
          }
        }
        .project__img--overlay {
          position: absolute;
          top: 0;
          bottom: 0;
          left: 0;
          right: 0;
          background: rgba(18, 0, 47, 0.6);
          color: #fff;
          visibility: hidden;
          opacity: 0;

          .project__content {
            margin: 3em 1em;

            p {
              text-align: justify;
            }

            .project__button {
              display: inline-block;
              color: #fff;
              background-color: $pink;
              padding: 0.4em 0.8em;
              border-radius: 0.5em;
              text-decoration: none;
              text-transform: uppercase;
              font-weight: 700;
            }
          }
        }

        &:hover .project__img--overlay {
          visibility: visible;
          opacity: 1;
        }
      }
    }
    .project__button__container {
      text-align: center;

      .projects__button {
        display: inline-block;
        color: #fff;
        background-color: $pink;
        padding: 1em 1.5em;
        margin: 0.8em;
        border-radius: 0.5em;
        text-decoration: none;
        text-transform: uppercase;
        font-weight: 700;
      }
    }
  }
}
</style>
