<script>
  import ayoReception from "../../lib/images/misc/ayo_office_img_6397.webp";
</script>

<div id="services-page">
  <h1>Services</h1>
  <section id="service-list-section">
    <div id="service-list">
      <ul>
        <li>
          <a href="/services/osteopathy">Osteopathy</a>
        </li>
        <li>
          <a href="/services/acupuncture">Medical Acupuncture</a>
        </li>
        <li>
          <a href="/services/dse">DSE Workstation Assessment</a>
        </li>
        <li>
          <a href="/services/clinic-visit">Clinic Visit</a>
        </li>
      </ul>
    </div>
    <img src={ayoReception} alt="ayo in office" />
  </section>
</div>

<style lang="scss">
  @use "../../styles/base";

  #services-page {
    @media (max-width: 450px) {
      padding-bottom: 0px;
      img {
        display: none;
      }
      #service-list {
        div:first-of-type {
          padding-bottom: base.$padding-bottom;
        }
      }
      ul {
        li {
          text-align: center;
        }
      }
    }
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding-bottom: 50px;
    h1 {
      text-align: center;
      padding-bottom: 50px;
      font-size: base.$title;
    }

    #service-list-section {
      padding-left: base.$padding-left;
      padding-right: base.$padding-right;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      img {
        padding-left: base.$padding-left;
        padding-right: base.$padding-right;
      }
      #service-list {
        padding-left: base.$padding-left;
        padding-right: base.$padding-right;
        padding-bottom: base.$padding-bottom;
        h2 {
          color: base.$ayoosteogreen;
          font-size: base.$intro-text;
          padding-bottom: base.$padding-bottom;
        }
        ul {
          li {
            font-size: 30px;
            padding-bottom: 30px;
            list-style-type: none;
            a {
              text-decoration: none;
              color: base.$ayoosteoblue;
            }
            a:hover {
              color: base.$ayoosteogreen;
              text-decoration: underline;
            }
          }
        }
        div:first-of-type {
          padding-bottom: base.$padding-bottom;
          text-align: center;
        }
      }
    }
  }
</style>
