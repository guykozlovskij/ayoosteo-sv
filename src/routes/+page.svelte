<script>
  import new1 from "../lib/images/misc/new1.png?enhanced";
  import gocRegistration from "../lib/images/certification/AyoO9396.jpg?enhanced";
  import goc from "..//lib/images/certification/AyoO9396.jpg?enhanced";
  import ioMembership from "../lib/images/certification/iO-Member-logo-Digital.jpg?enhanced";
</script>

<section id="home-intro-section">
  <enhanced:img src={new1} alt="ayo profile" class="home-ayo-profile-image" />
  <div class="home-intro-text">
    <h1 id="ayo-title">Ayo Kozlovskij</h1>
    <h2>Osteopath, Naturopath and Health Coach</h2>
    <p>
      Hi, I’m Ayo, and I WANT to help you take charge of your health! With years
      of clinical experience, I have seen firsthand how overwhelming health
      advice can be—especially with all the conflicting information out there.
      My mission? To simplify the process, cut through the noise, and guide you
      toward sustainable habits that fit your busy life.
      <br class="longer-br" />
      I work with people struggling with migraines, chronic pain, low energy, or
      a new health diagnosis. Maybe your blood test results weren’t great, or you
      just want to feel healthier and more in control. Whatever your journey, I’m
      here to support you every step of the way!
      <br class="longer-br" />
      I offer online consultations worldwide, so no matter where you are, we can
      work together to improve your health.
    </p>
  </div>
</section>

<section id="service-definitions">
  <div id="service-1">
    <h2>Health Coaching</h2>
    <p>
      Health coaching is all about empowering you to take control of your
      well-being in a way that feels doable and sustainable. From nutrition and
      exercise to sleep, stress, and overall wellness, it’s about finding what
      works for you. With personalised guidance and support, you’ll build habits
      that not only improve your health but actually stick—so you can feel your
      best for the long run!
    </p>
    <div class="button-green-div services-button">
      <a class="button-green" href="/services/health-coaching">Learn More</a>
    </div>
  </div>
  <div id="service-2">
    <h2>Osteopathy and Medical Acupuncture</h2>
    <p>
      As an osteopath, I take a whole-body approach to treating musculoskeletal
      issues, from back and joint pain to headaches, muscle aches, and sports
      injuries. I also provide tailored advice, health screenings, and referrals
      to support overall well-being. <span style="color: white; text-decoration: underline;">However, I am currently not offering
      osteopathy and medical acupuncture services at this time.</span>
    </p>
    <div class="button-green-div services-button">
      <a class="button-green" id="blue-button" href="/services/osteopathy"
        >Learn More</a
      >
    </div>
  </div>
</section>

<section id="about-certification">
  <div>
    <div id="certification-text">
      <span>I am a registered member of:</span>
    </div>
    <ul>
      <li>
        General Osteopathic Council – Membership number <span
          class="membership-number">9396</span
        >
      </li>
      <li>
        Institute of Osteopathy – Membership number <span
          class="membership-number">107031</span
        >
      </li>
      <li>
        British Medical Acupuncture Society – Membership number <span
          class="membership-number">37243</span
        >
      </li>
    </ul>
  </div>
</section>

<div id="memberships">
  <enhanced:img src={goc} alt="ayo GOC registration" />
  <enhanced:img
    id="io-membership"
    src={ioMembership}
    alt="IO membership logo />"
  />
</div>

<style lang="scss">
  @use "../styles/base";

  html {
    scroll-behavior: smooth;
  }

  #ayo-title {
    text-transform: uppercase;
  }

  #home-intro-section {
    padding-bottom: 100px;
    display: flex;
    justify-content: center;
    flex-direction: row;
    flex-wrap: wrap;
    .home-ayo-profile-image {
      max-width: 450px;
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      padding-bottom: base.$padding-bottom;
      height: auto;
      width: 100%;
    }

    .home-intro-text {
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      h1 {
        text-align: center;
        padding-bottom: base.$padding-bottom;
        font-size: base.$title;
        color: #297d2d;
      }
      h2 {
        max-width: 380px;
        text-align: center;
        padding-bottom: base.$padding-bottom;
        font-size: base.$intro-text;
      }
      p {
        line-height: base.$article-line-height;
        max-width: base.$paragraph;
        padding-bottom: base.$padding-bottom;
        font-size: base.$text-regular;
        text-align: justify;
        text-justify: inter-word;
      }
    }

    #goc-registration {
      width: 180px;
      height: auto;
    }
  }

  #home-scroll-section {
    background-color: base.$ayoosteoblue;
    height: 300px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    h2 {
      text-align: center;
      display: flex;
      padding-bottom: base.$padding-bottom;
      font-weight: normal;
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      color: white;
      font-size: base.$intro-text;
    }
    div {
      display: flex;
    }
  }

  #service-definitions {
    .services-button {
      padding-top: 50px;
      padding-bottom: 10px;
    }
    #blue-button {
      background-color: base.$ayoosteoblue;
    }
    h2 {
      color: white;
      max-width: 380px;
      text-align: center;
      padding-bottom: base.$padding-bottom;
      font-size: base.$intro-text;
      height: 85px;
    }
    line-height: base.$article-line-height;
    font-size: base.$text-regular;
    text-align: justify;
    text-justify: inter-word;
    display: flex;
    flex-direction: row;
    @media (max-width: 800px) {
      flex-direction: column;
    }
    #service-1 {
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      flex-wrap: wrap;
      padding-top: 50px;
      padding-bottom: 50px;
      background-color: base.$ayoosteoblue;
      p {
        color: white;
        max-width: 550px;
        padding-left: base.$padding-left;
        padding-right: base.$padding-right;
      }
    }
    #service-2 {
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding-top: 50px;
      padding-bottom: 50px;
      background-color: base.$ayoosteogreen;
      p {
        color: white;
        max-width: 550px;
        padding-left: base.$padding-left;
        padding-right: base.$padding-right;
      }
    }
  }

  #about-certification {
    #certification-text {
      padding-bottom: base.$padding-bottom;
    }
    padding-top: 60px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    flex-wrap: wrap;
    padding-left: base.$padding-left;
    padding-right: base.$padding-right;
    display: flex;
    align-items: center;
    justify-content: center;
    h2 {
      padding-bottom: base.$padding-bottom;
      font-size: 40px;
      color: base.$ayoosteoblue;
    }
    p {
      line-height: base.$article-line-height;
      max-width: base.$paragraph;
      padding-bottom: base.$padding-bottom;
      font-size: base.$text-regular;
      text-align: justify;
      text-justify: inter-word;
      @media (max-width: 450px) {
        text-align: start;
      }
    }
    span {
      padding-bottom: base.$padding-bottom;
      font-size: base.$text-regular;
      color: base.$ayoosteoblue;
      padding-bottom: base.$padding-bottom;
      margin-top: 500px;
    }
    ul {
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      padding-bottom: 50px;
      list-style-position: inside;
      li {
        font-size: base.$text-regular;

        padding-bottom: 10px;
      }
    }
    .membership-number {
      font-weight: bold;
      color: black;
    }
  }

  #memberships {
    padding-bottom: 60px;
    img {
      height: auto;
    }
  }

  .longer-br {
    content: "";
    margin: 2em;
    display: block;
    font-size: 24%;
  }
</style>
