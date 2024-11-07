<section id="contact-component">
  <div>
    <h2>Have any questions about my services?</h2>
  </div>
  <h1>Contact Me</h1>
  <p>Osteopath and Medical Acupuncturist. Based in Thurrock and Havering.</p>
  <div id="contact-details">
    <div class="button-green-div">
      <a class="button-green" href="mailto: ayoosteo@gmail.com"><i class="fas fa-envelope"></i>ayoosteo@gmail.com</a>
    </div>
  </div>
</section>

<style lang="scss">
  @use "../../styles/base";

  #contact-component {
  width: 100%;
  background-color: base.$ayoosteoblue;
  height: 550px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding-left: base.$padding-left;
  padding-right: base.$padding-right;
  h2 {
    font-size: base.$intro-text;
    font-weight: normal;
    padding-bottom: base.$padding-bottom;
    text-align: center;
    color: rgb(255, 255, 255);
  }
  h1 {
    color: rgb(255, 255, 255);
    font-size: base.$title;
    padding-bottom: base.$padding-bottom;
  }
  p {
    color: rgb(255, 255, 255);
    font-size: base.$text-regular;
    max-width: 500px;
    text-align: center;
    padding-bottom: base.$padding-bottom;
  }
  #contact-details {
    a {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-bottom: 20px;
    }
  }
}
</style>