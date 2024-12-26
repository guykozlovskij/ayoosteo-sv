<section id="contact-component">
  <div>
    <h1>Contact Me</h1>
    <h2>
      Interested in my services?
      <br>
      Get in touch for
      a free discovery call.
    </h2>
  </div>
  <div id="contact-details">
    <div class="button-green-div">
      <a class="button-green" href="mailto: ayoosteo@gmail.com">
        <i class="fas fa-envelope"></i>
        ayoosteo@gmail.com
      </a>
    </div>
  </div>
</section>

<style lang="scss">
  @use "../../styles/base";

  #contact-component {
    text-align: center;
    width: 100%;
    background-color: base.$ayoosteoblue;
    height: 450px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding-left: base.$padding-left;
    padding-right: base.$padding-right;
    h2 {
      font-size: base.$intro-text;
      font-weight: normal;
      padding-bottom: 40px;
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
