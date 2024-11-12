<script>
  import logo from "$lib/images/logos/ayoosteo-logo.png";
</script>

<nav>
  <a href="/">
    <img id="ayoosteo-logo" src={logo} alt="ayo osteo logo">
  </a>
  <a href="/">
    <div id="ayoosteo-alt">
      <span id="ayoosteo-alt-1">A</span>
      <span id="ayoosteo-alt-2">O</span>
    </div>
  </a>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About Me</a></li>
    <li><a href="/services">Services</a></li>
    <li><a href="/blogs">Blog</a></li>
  </ul>
  <div id="hamburger-menu">
    <input id="menu__toggle" type="checkbox" />
    <label class="menu__btn" for="menu__toggle">
      <span></span>
    </label>
    <ul class="menu__box">
      <li><a class="menu__item" href="/">Home</a></li>
      <li><a class="menu__item" href="/about">About Me</a></li>
      <li><a class="menu__item" href="/services">Services</a></li>
      <li><a class="menu__item" href="/blogs">Blog</a></li>
    </ul>
  </div>
</nav>

<style lang="scss">
  @use "../../styles/base";

  nav {
    z-index: 2;
    a {
      text-decoration: none;
    }
    width: 100%;
    top: 0;
    position: fixed;
    box-shadow: 2px 2px 6px rgba(0, 0, 0, 0.4);
    height: 100px;
    display: flex;
    align-items: center;
    margin-bottom: 50px;
    font-size: larger;
    background-color: base.$navcolor;
    #ayoosteo-alt {
      display: none;
    }
    img {
      max-height: 80px;
      padding-bottom: 5px;
      padding-left: 15px;
    }
    ul {
      display: flex;
      margin-left: auto;
      li {
        list-style-type: none;
        letter-spacing: 1px;
        padding-right: 30px;
        a {
          text-decoration: none;
        }
      }
      a:hover {
        color: base.$ayoosteogreen;
        text-decoration: underline;
      }
    }
    @media (max-width: 500px) {
      #hamburger-menu {
        display: block;
      }
      ul {
        display: none;
      }
      height: 50px;
      img {
        display: none;
      }
      #ayoosteo-alt {
        padding-left: 20px;
        padding-right: 20px;
        font-size: 25px;
        display: block;
        span {
          font-family: "Times New Roman", Times, serif;
        }
        #ayoosteo-alt-1 {
          color: base.$ayoosteogreen;
        }
        #ayoosteo-alt-2 {
          color: base.$ayoosteoblue;
        }
      }
    }
  }

  #hamburger-menu {
    display: none;
    #menu__toggle {
      opacity: 0;
    }
    #menu__toggle:checked + .menu__btn > span {
      transform: rotate(45deg);
    }
    #menu__toggle:checked + .menu__btn > span::before {
      top: 0;
      transform: rotate(0deg);
    }
    #menu__toggle:checked + .menu__btn > span::after {
      top: 0;
      transform: rotate(90deg);
    }
    #menu__toggle:checked ~ .menu__box {
      left: 0 !important;
    }
    .menu__btn {
      position: fixed;
      top: 25px;
      right: 20px;
      width: 26px;
      height: 26px;
      cursor: pointer;
      z-index: 1;
    }
    .menu__btn > span,
    .menu__btn > span::before,
    .menu__btn > span::after {
      display: block;
      position: absolute;
      width: 100%;
      height: 2px;
      background-color: #303030;
      transition-duration: 0.25s;
    }
    .menu__btn > span::before {
      content: "";
      top: -8px;
    }
    .menu__btn > span::after {
      content: "";
      top: 8px;
    }
    .menu__box {
      display: block;
      // text-align: center;
      position: fixed;
      top: 0;
      left: -100%;
      width: 300px;
      height: 100%;
      margin: 0;
      padding: 80px 0;
      list-style: none;
      background-color: base.$ayoosteoblue;
      box-shadow: 2px 2px 6px rgba(0, 0, 0, 0.4);
      transition-duration: 0.25s;
    }
    .menu__item {
      display: block;
      padding: 12px 24px;
      color: rgb(255, 255, 255);
      font-size: 25px;
      font-weight: 600;
      text-decoration: none;
      transition-duration: 0.25s;
    }
  }
</style>