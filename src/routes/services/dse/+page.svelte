<script>
  import workstation from "../../../lib/images/misc/computer-infographic.jpeg";
</script>

<svelte:head>
  <title>Workstation & DSE Assessments | Ergonomic Health | Ayoosteo</title>
  <meta name="description" content="In-depth workstation assessments to improve posture, reduce discomfort, and comply with DSE regulations for healthier working environments." />
</svelte:head>


<section class="service-display-page">
  <h1 class="service-title">Workstation Assessment</h1>
  <h2>
    Many musculoskeletal pain cases are caused by either a poorly designed
    workstation setup or the improper use of a good workstation.
  </h2>
  <div class="services-text">
    <p id="dse1">
      For many of us, a significant portion of our day is spent behind a
      computer screen.
    </p>
    <p id="dse2" class="italic">Who needs to be assessed:</p>
    <ul>
      <li>Anyone who works behind a desk for an hour or more at a time</li>
      <li>Anyone experiencing discomfort/pain while working</li>
    </ul>
    <div id="computer-infographic">
      <img src={workstation} alt="computer infographic" />
    </div>
    <h2 id="dse4">Why choose me:</h2>
    <ul>
      <li>
        I am a qualified osteopath with specialist ergonomic training and
        in-depth knowledge of biomechanics, posture, and musculoskeletal issues.
      </li>
      <li>
        I provide practical, tailored solutions and educate you on posture and
        chair adjustments.
      </li>
      <li>
        I optimise the use of available equipment, your environment, and work
        routines to minimise risks.
      </li>
      <li>
        I offer personalised exercises and stretches to address specific issues.
      </li>
      <li>
        My recommendations are clear, actionable, and based on thorough
        assessment findings.
      </li>
    </ul>
    <div id="dse-services">
      <div>
        <h4>Book a 60 minute online assessment - £80</h4>
        <p class="dse-bold">
          Includes a full report within 1-2 days and a follow up call to check
          in.
        </p>
        <div id="contact-details">
          <div class="button-green-div">
            <a class="button-green" href="mailto: ayoosteo@gmail.com">
              <i class="fas fa-envelope"></i>
              Book Now
            </a>
          </div>
        </div>
        <span>Assessment can be carried out in person at an aditional cost</span
        >
      </div>
    </div>
  </div>
</section>

<style lang="scss">
  @use "../../../styles/base";
  @use "../../../styles/services";

  h4 {
    font-size: 25px;
    padding-bottom: 20px;
  }
  #dse-services {
    background-color: base.$ayoosteoblue;
    padding: 30px;
    margin-bottom: 30px;
    border: 6px solid base.$ayoosteogreen;
    background-color: base.$ayoosteoblue;
    border-radius: 10px;
    h4,
    h3,
    p,
    span {
      color: whitesmoke !important;
    }
  }

  #contact-details {
    text-align: center;
    padding-top: 10px;
    padding-bottom: 40px;
    a {
      margin-bottom: 20px;
      width: 230px;
    }
  }
</style>
