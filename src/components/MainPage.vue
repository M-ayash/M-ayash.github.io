<template>
  <section class="main-page" id="main-page">
    <div class="main-content">
      <div class="page-title">
        <h1><span></span>Developer</h1>
        <p>
          // Enthousiaste web developer with frontend experience Knowledge of
          HTML, CSS, Javascript, PHP, Wordpress and Vuejs. en Hardware .opzoek
          naar een leuke baan waarin ik verder kan ontwikkelen samen met andere
          ICT collega's . //
        </p>
      </div>
      <div class="right-block">
        <h2>Hi, I am Mohammad <i class="hand-wave-emoji"></i></h2>
        <h3>Front-end Developer</h3>
        <div class="right-block-p">
          <div class="right-block-circles">
            <span></span><span></span><span></span>
          </div>
          <p>
            //<br />
            I am a web developer with frontend experience Knowledge of HTML,
            CSS, Javascript, PHP, Wordpress and Vuejs.
            <br />
            //
          </p>
        </div>
      </div>
      <div class="laptop-block">
        <div class="laptop-screen">
          <img src="@/assets/img/code1.png" alt="code" />
          <div class="top-screen"><span></span><span></span><span></span></div>
          <p class="text-screen">
            <i class="hand-wave-emoji"></i> I am <br />
            Mohammad Ayash
          </p>
          <div class="bottom-screen">
            <p></p>
            <p></p>
          </div>
        </div>
        <div class="laptop-keyboard">
          <img src="@/assets/img/laptop-keyboard.jpg" alt="keyboard" />
        </div>
      </div>
      <div>
        <button
          class="btn text-white border border-white btn-scroll-top"
          @click="goto('main-page')"
          title="go top"
        >
          &#8679;
        </button>
      </div>
    </div>
  </section>
</template>
<script>
  export default {
    methods: {
      goto(id) {
        var element = document.getElementById(id);
        element.scrollIntoView({
          behavior: "smooth",
        });
      },
      //
    },
  };
</script>
<style>
  .main-page {
    min-height: 100vh;
    min-width: 100%;
    padding-top: 30px;
  }

  .social-icons a {
    padding: 10px;
    text-decoration: none;
    font-size: 20px;
    color: #f7f7f7;
    text-shadow: -1px 0 black, 0 1px black, 1px 0 black, 0 -1px black;
  }
  .btn-contact {
    font-size: 20px;
    padding: 20px 50px;
    background-color: #81a9b5 !important;
    color: #fff !important;
  }
  .btn-scroll-top {
    position: fixed;
    padding: 20px;
    bottom: 5px;
    right: 5px;
    border-radius: 10px;
  }
  .laptop-block {
    width: 60%;
    margin: 0 auto;
    width: 400px;
  }
  .laptop-screen {
    background-color: #fff;
    border: 15px solid #000;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
  }
  .laptop-screen img {
    width: 100%;
  }
  .laptop-screen .text-screen {
    text-align: center;
    font-size: 2em;
    font-weight: bold;
    margin: auto;
    color: rgb(34, 32, 32);
  }
  i.hand-wave-emoji {
    display: inline-block;
    width: 1em;
    height: 1em;
    background: url(/src/assets/img/wave-hand-emogji.png) no-repeat;
    background-position: center;
    background-size: cover;
  }
  .laptop-screen .top-screen {
    overflow: auto;
  }
  .laptop-screen .top-screen * {
    height: 10px;
    background-color: #dddddd;
    width: 40px;
    float: right;
    margin: 10px;
    border-radius: 2px;
  }
  .laptop-screen .top-screen :first-child {
    float: left;
    width: 50px;
  }
  .laptop-screen .bottom-screen * {
    height: 5px;
    background-color: #dddddd;
    width: 60%;
    margin: 10px auto;
    border-radius: 10px;
  }
  .laptop-screen .bottom-screen :last-child {
    width: 40%;
    margin-bottom: 20px;
  }
  .laptop-keyboard {
    transform: translateX(22px);
  }
  .laptop-keyboard img {
    width: 100%;
    height: 120px;
    transform: skew(20deg);
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    border-bottom: 10px solid #000;
  }
  .right-block {
    position: absolute;
    width: 300px;
    overflow: auto;
    border: 4px solid #000;
    border-radius: 5%;
    background-color: #323232;
    padding: 10px;
    top: 35%;
    left: 90%;
  }
  .right-block h2 {
    color: #fff;
    font-size: 1.5em;
    text-align: center;
  }
  .right-block h3 {
    color: #fff;
    font-size: 1.2em;
    text-align: center;
  }
  .right-block-p {
    color: #41dd16;
    background-color: #3d3d3d;
    padding: 5px;
  }
  .right-block .right-block-circles span {
    border-radius: 50%;
    display: inline-block;
    margin: 2px;
    width: 7px;
    height: 7px;
  }
  .right-block .right-block-circles span:nth-child(1) {
    background-color: #ff2929;
  }
  .right-block .right-block-circles span:nth-child(2) {
    background-color: #f4ec1e;
  }
  .right-block .right-block-circles span:nth-child(3) {
    background-color: #56ff13;
  }
  @media (max-width: 850px) {
    .main-page {
      margin: 5px;
      padding: 40px;
      flex-direction: column;
    }
    .main-content {
      display: block;
      flex-direction: column;
      width: 90%;
    }

    .btn-contact {
      font-size: 20px;
    }
    .main-img {
      display: block;
      text-align: center;
    }
    .main-img img {
      width: 100%;
    }
    .right-block {
      position: static;
      width: 80%;
      margin: 20px auto;
    }
    .laptop-block {
      width: 80%;
    }
  }
  @media (max-width: 576px) {
    .main-page {
      padding: 20px;
      padding-top: 6em;
    }
  }

  @media (max-width: 360px) {
    .main-page {
      padding: 10em 0;
    }
    .right-block,
    .laptop-block {
      width: 100%;
    }
  }
</style>
