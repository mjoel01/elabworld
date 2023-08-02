<script>
import { ref } from "vue";
import navbar from "./components/navbar.vue";

export default {
  components: { navbar },
  setup() {},
};
</script>

<template>
  <navbar />
  <section class="hero">
    <h1 class="hero-heading">
      world e-lab tackling
      <br />the Grand Challenge <br />for Education.
    </h1>

    <div class="hero-img-wrapper">
      <div class="hero-subtitle">
        <p>aLU campus.</p>
        <p>kigali, rwanda</p>
      </div>

      <div class="hero-img"></div>
    </div>
  </section>

  <section class="mission">
    <main class="mission-main">
      <div class="mission-main-wrapper">
        <h4>our mission statement is</h4>
        <p>
          To increase student retention rates in Kenyan schools by
          <br />mentoring students and creating awareness of education
          <br />importance
        </p>
      </div>
      <div class="mission-main-wrapper">
        <h4>the Problem Statement stated</h4>
        <p>
          Latest report by the Kenya National Bureau of statistics
          <br />shows that,6.5 percent primary girls drop out of school
          <br />hence ending up getting pregnant. How can creating
          <br />awareness on education importance curb this problem?
        </p>
      </div>

      <div class="mission-main-wrapper">
        <h4>the solution Statement & stake holders</h4>
        <p>
          To deploy Mobile Education Units to reach girls in remote
          <br />areas who will be equipped with education materials, <br />audio
          visuals resources and tutors, and the stake <br />holders are parents,
          schools and primary school girls
        </p>
      </div>
    </main>

    <footer class="footer-mission">
      <p>worle-lab thinktank</p>
      <p>2023</p>
    </footer>
  </section>
  <section class="gallery">
    <main class="gallery-main">
      <div class="gallery-img-1"></div>
      <div class="gallery-img-2"></div>
      <div class="gallery-img-3"></div>
      <div class="gallery-img-4"></div>
      <div class="gallery-img-5"></div>
    </main>
    <footer class="footer-gallery">
      <p>worle-lab thinktank</p>
      <p>2023</p>
    </footer>
  </section>
  <section class="challanges">
    <div class="challange-wrapper">
      <h1>challenge one recap</h1>
      <div class="challange-video-wrapper">
        <video
          src="./assets/imgs/WhatsApp Video 2023-07-31 at 10.09.49 AM.mp4"
          controls
        ></video>
      </div>
    </div>
    <div class="challange-wrapper">
      <h1>challenge two recap</h1>
      <video
        controls
        src="./assets/imgs/WhatsApp Video 2023-07-31 at 10.09.50 AM.mp4"
      ></video>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.hero {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 9.6rem;
  padding: 3.2rem;

  .hero-heading {
    font-size: 4rem;
    text-transform: uppercase;
    text-align: center;
    align-self: center;
  }

  .hero-img-wrapper {
    // align-items: center;
    display: flex;
    flex-direction: column;
    gap: 1.2rem;

    .hero-subtitle {
      width: 100%;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      p {
        font-size: 1.6rem;
        text-transform: capitalize;
      }
    }
    .hero-img {
      width: 100%;
      height: 72rem;
      background: linear-gradient(rgb(0, 0, 0, 0.55), rgb(0, 0, 0, 0.55)),
        url(./assets/imgs/e-lab-background.png);
      background-repeat: no-repeat;
      background-size: cover;
    }
  }
}

.mission {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 3.2rem;
  height: 100vh;

  .mission-main {
    display: flex;
    flex-direction: column;
    gap: 3.2rem;
    align-self: flex-end;

    .mission-main-wrapper {
      display: flex;
      flex-direction: column;
      gap: 1.2rem;

      h4 {
        font-size: 2rem;
        text-transform: capitalize;
        align-self: flex-end;
      }
      p {
        font-size: 2rem;
        color: #313131;
        text-transform: capitalize;
      }
    }
  }

  .footer-mission {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    p {
      font-size: 1.6rem;
      text-transform: uppercase;
    }
  }
}

.gallery {
  display: flex;
  flex-direction: column;
  gap: 3.2rem;
  height: 100vh;
  padding: 3.2rem;

  .gallery-main {
    height: 100%;
    width: 100%;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, 1fr);
    row-gap: 3.2rem;
    column-gap: 3.2rem;

    .gallery-img-1 {
      grid-row: 1/1;
      grid-column: 1/1;
      background: linear-gradient(rgb(0, 0, 0, 0.55), rgb(0, 0, 0, 0.55)),
        url(./assets/imgs/1ce7c4e8687ee6cdd7caaedac30e1c83.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }

    .gallery-img-2 {
      grid-row: 2/-1;
      grid-column: 1/1;
      background: linear-gradient(rgb(0, 0, 0, 0.55), rgb(0, 0, 0, 0.55)),
        url(./assets/imgs/273f8eb6ed669c9bcb89e2f25f49432c.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }

    .gallery-img-3 {
      grid-row: 1/-1;
      grid-column: 2/3;
      background: linear-gradient(rgb(0, 0, 0, 0.55), rgb(0, 0, 0, 0.55)),
        url(./assets/imgs/be00b58659693385bd6c45353fbf58b6.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }

    .gallery-img-4 {
      grid-row: 1/2;
      grid-column: 3/-1;
      background: linear-gradient(rgb(0, 0, 0, 0.55), rgb(0, 0, 0, 0.55)),
        url(./assets/imgs/blog_kenyanschool669.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }

    .gallery-img-5 {
      grid-row: 2/-1;
      grid-column: 3/-1;
      background: linear-gradient(rgb(0, 0, 0, 0.55), rgb(0, 0, 0, 0.55)),
        url(./assets/imgs/Kenyagirlducation.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }
  }

  .footer-gallery {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    p {
      font-size: 1.6rem;
      text-transform: uppercase;
    }
  }
}
.challanges {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 9.6rem;

  .challange-wrapper {
    display: flex;
    flex-direction: column;
    gap: 1.6rem;
    align-self: center;

    h1 {
      align-self: center;
      font-size: 4.8rem;
      text-transform: capitalize;
    }

    video {
      width: 70vw;
      height: 55vw;
      // background-color: rgb(0, 0, 0, 0.5);
      // align-self: c;
    }
  }
}
</style>
