<script>
  import new2 from "../../lib/images/misc/new2.png";
  import goc from "../../lib/images/certification/AyoO9396.jpg";
  import ioMembership from "../../lib/images/certification/iO-Member-logo-Digital.jpg";
</script>

<section id="about-page">
  <div id="about-profile-image">
    <img src={new2} alt="ayo profile" />
    <h2>M.Ost, DO, ND</h2>
  </div>
  <section id="about-section">
    <h1>About Me</h1>
    <h2>AYO KOZLOVSKIJ</h2>
    <p>
      I graduated from the British College of Osteopathic Medicine with a
      Masters in Osteopathy and a Diploma in Naturopathy.
    </p>
    <p>
      As an osteopath, I take a patient centred approach in working together
      with you to help you recover from pain or injury, achieve optimal health
      and altogether have an improved quality of life. I often combine
      osteopathic techniques with advice on exercises, ergonomics, dietary
      changes, wellness strategies and along the way helping you to understand
      the problem and how to prevent it from recurring.
    </p>
    <p>
      I have experience of working with a wide spectrum of patients, as young as
      newborns, adolescents, adults and geriatric patients.
    </p>
    <p>
      Additionally, I hold qualifications in Medical Acupuncture, having
      received training from the British Medical Acupuncture Society. I have
      also worked as an osteopathic technique tutor and a practice educator at
      The British College of Osteopathic Medicine and at the University College
      of Osteopathy in London.
    </p>
    <p>
      Outside of work I enjoy defeating my husband at badminton and indulging in
      activities such as yoga and body weight exercises.
    </p>
  </section>
</section>

<section id="about-certification">
  <div>
    <div id="certification-text">
      <h2>Certification</h2>
      <p>
        By law it is essential that I am registered with the General Osteopathic
        Council. This is to protect you as the patient. It is also essential
        that I have professional indemnity insurance.
      </p>
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
  <img src={goc} alt="ayo GOC registration" />
  <img id="io-membership" src={ioMembership} alt="IO membership logo />" />
</div>

<style lang="scss">
  @use "../../styles/base";

  #about-page {
    display: flex;
    justify-content: center;
    flex-direction: row;
    flex-wrap: wrap;
    display: flex;
    align-items: center;
    justify-content: center;
    padding-bottom: 50px;
    #about-section {
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
    }
    h1 {
      text-align: center;
      padding-bottom: base.$padding-bottom;
      font-size: base.$title;
    }
    h2 {
      text-align: center;
      padding-bottom: base.$padding-bottom;
      font-size: 40px;
      color: base.$ayoosteogreen;
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
  }

  #about-profile-image {
    max-width: 400px;
    padding-left: base.$padding-left;
    padding-right: base.$padding-right;
    padding-bottom: base.$padding-bottom;
    img {
      width: 100%;
      border-radius: 50%;
      filter: grayscale(100%);
      margin-bottom: base.$padding-bottom;
    }
    h2 {
      text-align: center;
      color: base.$ayoosteogreen;
    }
  }

  #about-certification {
    #certification-text {
      padding-bottom: base.$padding-bottom;
    }
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
</style>
