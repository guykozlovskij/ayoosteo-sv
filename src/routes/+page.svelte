<script>
  import new1 from "../lib/images/misc/new1.png";
  import gocRegistration from "../lib/images/certification/AyoO9396.jpg";
  import ayoReception from "../lib/images/misc/ayo-reception_e0c10b38-c6a9-4fa4-8923-745833add36e_1_201_a.webp";
</script>

<section id="home-intro-section">
  <div id="home-ayo-profile-image">
    <img src={new1} alt="ayo profile" />
  </div>
  <div class="home-intro-text">
    <h1>AYO KOZLOVSKIJ</h1>
    <h2>Osteopath and Medical Acupuncturist</h2>
    <p>
      Based in Thurrock and Havering. My passion is to help you to recover from
      pain, rehabilitate from injury and achieve great health. I provide a
      highly effective treatment to ensure that your symptoms improve in as few
      sessions as possible.
    </p>
    <img
      id="goc-registration"
      src={gocRegistration}
      alt="general osteopathic council registration no 9396"
    />
  </div>
</section>

<section id="home-scroll-section">
  <h2>What does an osteopath treat?</h2>
  <div class="button-green-div">
    <a class="button-green" href="/src/pages/services.html">View List</a>
  </div>
</section>

<section id="home-appointment-section">
  <div id="book-appointment-div">
    <img src={ayoReception} alt="ayo reception" />
    <div id="book-appointment-button" class="button-green-inverted-div">
      <a class="button-green-inverted" href="#contact-component"
        >Book an appointment</a
      >
    </div>
  </div>
  <div id="treatment-types-div">
    <div class="treatment">
      <h3>Osteopathy</h3>
      <p>Consultation and Treatment: 60 minutes</p>
      <p>Follow up: 30 minutes</p>
    </div>
    <div class="treatment">
      <h3>Osteopathy and Medical Acupuncture</h3>
      <p>Consultation and Treatment: 60 minutes</p>
      <p>Follow up: 45 minutes</p>
    </div>
    <div class="treatment">
      <h3>Home Visit</h3>
      <p>Consultation and Treatment: 60 minutes</p>
      <p>Follow up: 40 minutes</p>
    </div>
    <div class="treatment">
      <h3>Work Station Assessment</h3>
      <p>Basic or Complex Assessment</p>
      <p>30 Minutes to 1 hour</p>
    </div>
  </div>
  <hr class="solid" />
  <p id="registered-with">
    I am registered with most health insurers, including AXA-PPP, Vitality,
    Simply Health and many others (however, I am not linked with BUPA).
  </p>
</section>

<style lang="scss">
  @use "../styles/base";

  #home-intro-section {
    padding-bottom: 100px;
    display: flex;
    justify-content: center;
    flex-direction: row;
    flex-wrap: wrap;
    #home-ayo-profile-image {
      max-width: 450px;
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      padding-bottom: base.$padding-bottom;
      img {
        width: 100%;
      }
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

  #home-appointment-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    #book-appointment-div {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: row;
      flex-wrap: wrap;
      padding-bottom: 50px;
      @media (max-width: 600px) {
        // flex-direction: column-reverse;
        img {
          padding-bottom: 50px;
        }
      }
      button:hover {
        background-color: base.$ayoosteoblue;
      }
      img {
        height: 420px;
        padding-top: 50px;
        padding-left: 25px;
        padding-right: 25px;
      }
    }
    #treatment-types-div {
      font-size: 24px;
      padding-left: 25px;
      padding-right: 25px;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      .treatment {
        padding-left: 30px;
        padding-right: 30px;
        text-align: center;
        padding-bottom: 60px;
        h3,
        p {
          color: rgb(0, 105, 69);
        }
        h3 {
          padding-bottom: 15px;
          font-size: 24px;
        }
        p {
          padding-bottom: 15px;
        }
      }
    }
    #registered-with {
      padding-left: 25px;
      padding-right: 25px;
      padding-top: 40px;
      padding-bottom: 40px;
      text-align: center;
      max-width: 800px;
      font-size: 30px;
    }
  }
</style>
