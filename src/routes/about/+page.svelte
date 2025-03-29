<script>
  import new2 from "../../lib/images/misc/new2.jpg?enhanced";
  import goc from "../../lib/images/certification/AyoO9396.jpg?enhanced";
  import ioMembership from "../../lib/images/certification/iO-Member-logo-Digital.jpg?enhanced";
</script>

<section id="about-page">
  <div id="about-profile-image">
    <enhanced:img src={new2} alt="ayo profile" />
    <h2>AYO KOZLOVSKIJ</h2>
    <h2>M.Ost, DO, ND</h2>
  </div>
  <section id="about-section">
    <h1>About Me</h1>
    <p>
      I graduated from the British College of Osteopathic Medicine with a
      Masters in Osteopathy and a Diploma in Naturopathy. With nearly a decade
      of clinical experience, I have found my greatest joy in helping people
      feel their best by guiding them toward sustainable health changes—without
      the overwhelm!
    </p>
    <p>
      To expand my ability to support patients, I trained with the College of
      Naturopathic Medicine to become a certified Health Coach. As a
      whole-health professional, I specialise in lifestyle and behaviour change,
      empowering clients to take charge of their well-being. I believe in a
      patient-centred approach that respects each individual's unique
      experience, combining osteopathic and naturopathic principles with health
      coaching strategies.
    </p>
    <p>
      New patients often come to me feeling unsure of where to start in
      addressing their health concerns. My role is to help them navigate this
      journey by identifying priorities, setting realistic goals, and clarifying
      the steps needed to create meaningful, lasting progress. Whether it’s
      movement, nutrition, sleep, stress management, or overall wellness, my
      focus is on equipping my patients with the tools and confidence to reclaim
      control of their health—and, ultimately, their lives.
    </p>
    <p>
      A key part of my approach is recognising that each person’s path to
      well-being is different. I take a broad perspective, considering a range
      of lifestyle factors that can either support or undermine health. My aim
      is to serve as a non-judgmental ally, providing guidance, motivation, and
      education to help clients break through resistance and make sustainable
      choices that align with their whole-health potential.
    </p>
    <p>
      I have experience working with individuals of all ages, from newborns to
      seniors, tailoring my approach to suit their unique needs. In addition to
      my osteopathic practice, I hold a diploma in Medical Acupuncture and have
      taught at leading colleges in London.
    </p>
    <p>
      If you're looking for a holistic and supportive approach to your health,
      get in touch!
    </p>
    <p>
      <a href="#contact-placeholder">Contact me</a> here or view my sevices <a href="/services/health-coaching">here</a>.
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
  <enhanced:img src={goc} alt="ayo GOC registration" />
  <enhanced:img
    id="io-membership"
    src={ioMembership}
    alt="IO membership logo />"
  />
</div>
<div id="contact-placeholder"></div>

<style lang="scss">
  @use "../../styles/base";
  #about-page {
    a{
      color: base.$ayoosteoblue;
    }
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
      height: auto;
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

  #memberships {
    img {
      height: auto;
    }
  }
</style>
