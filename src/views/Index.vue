<template>
  <div class="wrapper">
    <parallax class="page-header header-filter" :style="headerStyle">
      <div class="md-layout">
        <div class="md-layout-item animate__animated animate__fadeIn">
          <div class="image-wrapper">
            <div class="brand">
              <h1 class="farmvi-logo">Farmvi</h1>
              <h3 style="line-height: 1;">
                Farmvi's mission is to make the life of farmers easier.<br />
                Empowering agriculture growers from the sky.
              </h3>
            </div>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised rounded-border">
      <md-card
        class="md-card md-card-principal mx-2"
        :style="backgroundCardStyle"
      >
        <md-card-content>
          <p class="font-weight-semibold text-white">
            Your field in your pocket
          </p>
          <h2 class="font-weight-bold text-green">*Plant the future_</h2>
          <p class="font-weight-semibold first-card-subt text-white">
            The main idea behind Farmvi is to simplify the agriculture
            decision-making process for farmers and to optimize their inputs.
            Smart farming, easy living.
          </p>
          <md-button class="md-round md-success">
            GET IT NOW
          </md-button>
        </md-card-content>
      </md-card>
      <div class="second-section text-center" :style="backgroundField">
        <img :src="phoneMockup" alt="Farmvi app" />
      </div>
      <div class="third-section text-center">
        <h2 class="font-weight-bold text-green">
          _Navigate your farm.
        </h2>
        <p class="md-subheading font-weight-semibold">
          The technology behind Farmvi is based on four premises
        </p>
        <div class="md-layout">
          <div class="md-layout-item md-size-25 md-small-size-50">
            <!-- :class="{ animate__jello: cardOneHovering }" -->
            <div
              class="md-card first-card information-pills background-green animate__animated"
              @mouseover="cardOneHovering = true"
              @mouseout="cardOneHovering = false"
            >
              <md-card-content class="information-pill-content">
                <p class="font-weight-semibold text-white">
                  Farmvi is for farmers
                </p>
              </md-card-content>
            </div>
          </div>
          <div class="md-layout-item md-size-25 md-small-size-50">
            <div class="md-card second-card information-pills background-green">
              <md-card-content class="information-pill-content">
                <p class="font-weight-semibold text-white">
                  Move from precision farming to smart farming
                </p>
              </md-card-content>
            </div>
          </div>
          <div class="md-layout-item md-size-25 md-small-size-50">
            <div class="md-card third-card information-pills background-green">
              <md-card-content class="information-pill-content">
                <p class="font-weight-semibold text-white">
                  Serve your specific needs, not a generic solution
                </p>
              </md-card-content>
            </div>
          </div>
          <div class="md-layout-item md-size-25 md-small-size-50">
            <div class="md-card fourth-card information-pills background-green">
              <md-card-content class="information-pill-content">
                <p class="font-weight-semibold text-white">
                  Maximize your potential with computer vision
                </p>
              </md-card-content>
            </div>
          </div>
        </div>
        <p class="md-subheading font-weight-semibold">
          We work closely with farmers and agricultural engineers to provide you
          with the most powerful and precise tool. And as for the plants, our
          development process to help you never stops.
        </p>
      </div>
      <div class="fourth-section">
        <div class="md-layout">
          <div class="md-layout-item md-size-100">
            <div class="md-card-title title-background">
              <h2 class="text-green font-weight-bold">
                Sm&#60;rt farming, <span class="text-white">easy</span> living_
              </h2>
            </div>
          </div>
        </div>
        <div class="md-layout flex-row-small">
          <div
            class="md-layout md-layout-item md-size-100 flex-no-wrap row-margin"
          >
            <div class="md-layout-item md-size-75 md-small-size-100">
              <div class="md-card background-effect">
                <md-card-content class="md-layout">
                  <div
                    class="img-box md-layout-item md-size-50 md-small-size-100"
                  >
                    <img :src="haveControlImg" alt="" />
                  </div>
                  <div
                    class="text-box md-layout-item md-size-50 md-small-size-100"
                  >
                    <h3 class="text-green align-self-left font-weight-bold">
                      Have control of your farm
                      <span class="text-white">from anywhere</span>
                    </h3>
                    <p class="font-weight-semibold text-white">
                      Farmvi is oriented to farmers, and all of its features are
                      built based on that premise. That means that we do not
                      provide raw data or generic solutions. We provide you with
                      the best of precision farming that you can use easily from
                      anywhere.
                    </p>
                    <md-button class="md-round white-transparent-button">
                      TRY WEB APP
                    </md-button>
                  </div>
                </md-card-content>
              </div>
            </div>
            <div class="md-layout-item md-size-25 md-small-hide">
              <div class="md-card background-custom-1"></div>
            </div>
          </div>
          <div class="md-layout md-layout-item md-size-100 flex-no-wrap">
            <div class="md-layout-item md-size-40 md-small-size-100">
              <div class="md-card background-brown">
                <md-card-content class="md-layout text-right">
                  <div class="md-layout-item md-size-100 flex-right">
                    <h3 class="text-green font-weight-bold align-right">
                      Compare yourself
                      <span class="text-white">to other farmers</span>
                    </h3>
                  </div>
                  <div class="img-text-box md-layout-item md-size-100">
                    <img :src="compareImg" alt="" />
                    <p
                      class="paragraph-fs text-white text-over-img font-weight-semibold"
                    >
                      Compare performance with your neighbors, share information
                      about extended problems, or just have an overview of the
                      whole area
                    </p>
                  </div>
                </md-card-content>
              </div>
            </div>
            <div class="md-layout-item md-size-20 md-small-size-50">
              <div class="md-card background-custom-2"></div>
            </div>
            <div class="md-layout-item md-size-40 md-small-size-100">
              <div class="md-card background-orange">
                <md-card-content class="md-layout text-right">
                  <div class="md-layout-item md-size-100 flex-right">
                    <h3
                      class="long-title text-green font-weight-bold align-right"
                    >
                      Try our
                      <span class="block-span text-white">
                        hyperresolution model
                      </span>
                    </h3>
                  </div>
                  <div class="img-text-box md-layout-item md-size-100">
                    <img :src="compareImg" alt="" />
                    <p
                      class="paragraph-fs text-white text-over-img font-weight-semibold"
                    >
                      Compare performance with your neighbors, share information
                      about extended problems, or just have an overview of the
                      whole area
                    </p>
                  </div>
                </md-card-content>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="fifth-section text-center">
        <h2>Get Farmvi</h2>
        <h3>Get our mobile App</h3>
        <p>
          Get the farmvi Mobile App and achieve complete control of your farm.
          farm. All the functionalities you were searching in the palm of your
          hand.
        </p>
        <div class="buttons">
          <md-button class="md-round white-transparent-button">
            <i class="material-icons">android</i>
            GET IT NOW
          </md-button>
          <md-button class="md-round white-transparent-button">
            <i class="material-icons">apple</i>
            GET IT NOW
          </md-button>
        </div>
        <h3>Or use our Web App</h3>
        <p>
          If you don't want to download the app, you can always try our desktop
          version
        </p>
        <div class="buttons">
          <md-button class="md-round white-transparent-button">
            GET IT NOW
          </md-button>
        </div>
      </div>
      <div class="sixth-section">
        <div class="md-layout-item md-size-100">
          <nav-pills></nav-pills>
        </div>
      </div>
      <div class="cards-section">
        <div class="md-layout">
          <div class="md-layout-item md-size-40 md-small-size-100">
            <div class="main-paragraph">
              <h2 class="font-weight-bold text-green">
                /Empowering agriculture grøwers from the sky_
              </h2>
              <p>
                Daily Earth data for farming solutions. Satellite images are to
                capture the interaction between the sun and your crops/soil.
                Something invisible for the human eye. Information is vital, and
                transforming these interactions into actionable tools helps
                farmers to optimize their farm management workflow.
              </p>
            </div>
          </div>
          <div class="md-layout-item md-size-60 md-small-size-100">
            <div class="md-layout">
              <div class="md-layout-item md-size-25 md-xsmall-size-50">
                <div class="md-card emp-cards">
                  <div class="background-image-card card-1">
                    <md-card-content>
                      <p class="font-weight-semibold">
                        You can record your activities,
                        <span class="text-orange font-weight-bold">
                          track your plants
                        </span>
                        or simply write notes
                      </p>
                    </md-card-content>
                  </div>
                  <div
                    class="background-image-card background-image-card--back background-green"
                  >
                    <md-card-content>
                      <p class="font-weight-semibold">
                        Every action you made is automatically registered in the
                        log system, so you can take a look at where and when.
                      </p>
                    </md-card-content>
                  </div>
                </div>
              </div>
              <div class="md-layout-item md-size-25 md-xsmall-size-50">
                <div class="md-card emp-cards">
                  <div class="background-image-card card-2">
                    <md-card-content>
                      <p class="font-weight-semibold">
                        <span class="text-orange font-weight-bold">
                          Satellite images
                        </span>
                        provide wide ranges of spatial and historical
                        information.
                      </p>
                    </md-card-content>
                  </div>
                  <div
                    class="background-image-card background-image-card--back background-green"
                  >
                    <md-card-content>
                      <p class="font-weight-semibold">
                        Differences in the reflectance captured along the time
                        are a highly successful tool for analyzing your crops.
                      </p>
                    </md-card-content>
                  </div>
                </div>
              </div>
              <div class="md-layout-item md-size-25 md-xsmall-size-50">
                <div class="md-card emp-cards">
                  <div class="background-image-card card-4">
                    <md-card-content>
                      <p class="font-weight-semibold">
                        You can use the
                        <span class="text-orange font-weight-bold">
                          anomaly maps
                        </span>
                      </p>
                    </md-card-content>
                  </div>
                  <div
                    class="background-image-card background-image-card--back background-green"
                  >
                    <md-card-content>
                      <p class="font-weight-semibold">
                        By using anomaly maps you can detect precisely when and
                        where there is an issue so you can take timely
                        decisions.
                      </p>
                    </md-card-content>
                  </div>
                </div>
              </div>
              <div class="md-layout-item md-size-25 md-xsmall-size-50">
                <div class="md-card emp-cards">
                  <div class="background-image-card card-3">
                    <md-card-content>
                      <p class="font-weight-semibold">
                        <span class="text-orange font-weight-bold">
                          Crop Management
                        </span>
                        is where satellite images can provide the most value.
                      </p>
                    </md-card-content>
                  </div>
                  <div
                    class="background-image-card background-image-card--back background-green"
                  >
                    <md-card-content>
                      <p class="font-weight-semibold">
                        They transmit instant information on the crops that
                        helps farmers for making easy and better agronomic
                        decisions.
                      </p>
                    </md-card-content>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- <div class="reviews-section">
            <div class="md-layout">
              <div class="md-layout-item md-size-100 mx-auto">
                <md-card>
                  <carousel
                    :per-page="1"
                    loop
                    :speed="700"
                    autoplay
                    :autoplay-timeout="5000"
                    :mouse-drag="false"
                    navigationEnabled
                    navigationNextLabel="<i class='material-icons'>keyboard_arrow_right</i>"
                    navigationPrevLabel="<i class='material-icons'>keyboard_arrow_left</i>"
                  >
                    <slide>
                      <div class="carousel-caption">
                        <h4>
                          <md-icon>location_on</md-icon>
                          Erl McGonagall, farmer, United States
                        </h4>
                        <p class="margin-x">
                          Farmvi spares me trips to the fields because I can
                          monitor a specific crop, check its condition every
                          week and take action. In my work, it's very important
                          to have a tool that offers satellite images. You check
                          the NDVI maps, see where the index is low, and head
                          out right away to check a specific site. The app also
                          shows how the index changes over time.
                        </p>
                      </div>
                      <img :src="carousel1" alt="carousel1" />
                    </slide>
                    <slide>
                      <div class="carousel-caption">
                        <h4>
                          <md-icon>location_on</md-icon>
                          Yellowstone National Park, United States
                        </h4>
                      </div>
                      <img :src="carousel2" alt="carousel2" />
                    </slide>
                    <slide>
                      <div class="carousel-caption">
                        <h4>
                          <md-icon>location_on</md-icon>
                          Yellowstone National Park, United States
                        </h4>
                      </div>
                      <img :src="carousel3" alt="carousel3" />
                    </slide>
                  </carousel>
                </md-card>
              </div>
            </div>
          </div> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Tabs from "./components/TabsSection";
import NavPills from "./components/NavPillsSection";
import "animate.css";
export default {
  components: {
    NavPills
  },
  name: "index",
  bodyClass: "index-page",
  props: {
    image: {
      type: String,
      default: require("@/assets/img/header-image.jpg")
    },
    orangeBackground: {
      type: String,
      default: require("@/assets/img/background-card.jpg")
    },
    fieldBackground: {
      type: String,
      default: require("@/assets/img/field.jpg")
    },
    phoneMockup: {
      type: String,
      default: require("@/assets/img/prototipo-1.png")
    },
    haveControlImg: {
      type: String,
      default: require("@/assets/img/prototipo-2.png")
    },
    logoImg: {
      type: String,
      default: require("@/assets/img/farmvi-logo.png")
    },
    compareImg: {
      type: String,
      default: require("@/assets/img/compare-2.png")
    },
    profile: {
      type: String,
      default: require("@/assets/img/profile.jpg")
    }
  },
  data() {
    return {
      firstname: null,
      email: null,
      password: null,
      leafShow: false,
      cardOneHovering: false,
      carousel1: require("@/assets/img/nature-2.jpg"),
      carousel2: require("@/assets/img/nature.jpg"),
      carousel3: require("@/assets/img/nature-3.jpg")
    };
  },
  // methods: {
  // },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.image})`
      };
    },
    backgroundCardStyle() {
      return {
        backgroundImage: `url(${this.orangeBackground})`
      };
    },
    backgroundField() {
      return {
        backgroundImage: `url(${this.fieldBackground})`
      };
    },
    signupImage() {
      return {
        backgroundImage: `url(${this.signup})`
      };
    }
  }
  // mounted() {
  //   this.leafActive();
  //   window.addEventListener("resize", this.leafActive);
  // },
  // beforeDestroy() {
  //   window.removeEventListener("resize", this.leafActive);
  // }
};
</script>
<style scoped lang="scss">
/* GENERICS */
.main {
  padding: 20px 10px;
}
.font-weight-bold {
  font-weight: bold;
}
.font-weight-semibold {
  font-weight: 500;
}
.text-white {
  color: #fff;
}
.text-green {
  color: #0a3939;
}
.text-orange {
  color: #ff9c03;
}
.background-green {
  background-color: #0a3939;
}
.background-orange {
  background-color: #ff9c03;
}
.background-effect {
  background-color: #ff9c03;
  background-size: 200% 200%;
  background-image: linear-gradient(
    -45deg,
    #c25721 0%,
    #c25721 10%,
    #ff9c03 51%,
    #ff9c03 100%
  );
  animation: AnimateBG 10s ease infinite;
}
@keyframes AnimateBG {
  0% {
    background-position: 50% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 50% 50%;
  }
}
.background-brown {
  background-color: #c25721;
}
.text-center {
  text-align: center;
}
.text-right {
  text-align: right;
}
.paragraph-fs {
  font-size: 1.2rem;
}
.margin-x {
  margin: 0 30px;
}
.white-transparent-button {
  background-color: transparent !important;
  border: solid 1px white;
  margin-bottom: 15px !important;
}
.white-transparent-button:hover {
  background-color: white !important;
  border: solid 1px white;
  color: #0a3939 !important;
}
.rounded-border {
  border-radius: 27px;
  overflow: hidden;
}
.farmvi-logo {
  font-size: 0px !important;
  background-image: url("../assets/img/farmvi-logo.png");
  margin-bottom: 25px;
  height: 111px;
  width: 100%;
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center;
}
/* FIRST SECTION */
.md-card-principal {
  text-align: center;
  margin: 10px auto;
  max-width: 1200px;
  height: 100%;
  display: block;
  background-position: center;
  background-size: cover;
  border-radius: 27px;

  // h2 {
  //   display: inline-block;
  //   overflow: hidden; /* Ensures the content is not revealed until the animation */
  //   border-right: .15em solid orange; /* The typwriter cursor */
  //   white-space: nowrap; /* Keeps the content on a single line */
  //   margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  //   animation:
  //     typing 3.5s steps(40, end),
  //     blink-caret .75s step-end infinite;
  // }
  // @keyframes typing {
  //   from { width: 0 }
  //   to { width: 290px }
  // }

  // /* The typewriter cursor effect */
  // @keyframes blink-caret {
  //   from, to { border-color: transparent }
  //   50% { border-color: green; }
  // }
}
.first-card-subt {
  max-width: 700px;
  margin: 15px auto;
}
.second-section {
  margin: 50px -10px;
  min-height: 400px;
  background-position: center;
  background-size: cover;
}
/*THIRD SECTION*/
.third-section {
  margin: 50px auto;
  max-width: 1000px;
  .md-card {
    height: 215px;
    display: flex;
  }
  .information-pills {
    background-repeat: no-repeat;
    background-position: 50% 25%;
  }
  .information-pill-content {
    height: 90px;
    width: 100%;
    padding: 0;
    align-content: center;
    align-self: flex-end;
    padding: 10px !important;
  }

  .first-card {
    background-image: url("../assets/img/corn.png");
  }
  .second-card {
    background-image: url("../assets/img/star.png");
  }
  .third-card {
    background-image: url("../assets/img/four-circles.png");
  }
  .fourth-card {
    background-image: url("../assets/img/satellite.png");
  }
}
.fourth-section {
  margin: 50px auto;
  max-width: 1300px;
  .title-background {
    background-image: url("../assets/img/background-with-icons-3.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
  }
  .row-margin {
    margin-bottom: 20px;
  }

  .md-card {
    margin: 10px auto;
    display: flex;

    .img-box {
      align-content: center;
      justify-content: center;
      display: flex;
    }
    .img-box img {
      max-height: 500px;
      width: auto;
      margin: auto;
      display: inline-block;
    }
    @media all and (max-width: 960px) {
      .img-box img {
        max-height: 200px;
      }
    }
  }
  .md-card-title {
    margin: 0 15px;
    text-align: center;
    height: 100%;
    display: flex;
    align-content: center;
    justify-content: center;
    border-radius: 25px;
  }
  .md-button {
    width: 100px;
  }
  .md-card-content {
    justify-self: center;

    h3 {
      max-width: 200px;
      align-self: center;
      justify-self: center;
    }

    .align-self-left {
      align-self: flex-start;
    }

    .long-title {
      max-width: 300px;
    }

    .block-span {
      display: block;
    }

    img {
      display: inline-block;
    }

    .flex-right {
      display: flex;
      justify-content: flex-end;
    }

    .text-box {
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .img-text-box {
      position: relative;
    }

    .text-over-img {
      position: absolute;
      top: 20px;
      right: 30px;
      width: 210px;
    }
    @media all and (max-width: 960px) {
      .text-over-img {
        position: relative;
        top: 0px;
        right: 0px;
        width: auto;
      }
    }
  }

  .background-custom-1 {
    background-image: url("../assets/img/design-resource.jpg");
    background-position: center;
    background-size: cover;
  }
  .background-custom-2 {
    background-image: url("../assets/img/design-resource-02.jpg");
    background-position: center;
    background-size: cover;
  }
}
/* FIFTH SECTION */
.fifth-section {
  height: 852px;
  background-image: url("../assets/img/mockups-background-3.png");
  background-position: center;
  background-size: cover;
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 20px -10px;
  padding: 0px 10px;

  h2 {
    font-size: 53px;
    font-weight: bold;
  }

  h3 {
    font-size: 30px;
    font-weight: bold;
  }

  p {
    font-size: 20px;
    max-width: 500px;
    margin: 0 auto;
  }

  .buttons {
    margin-top: 30px;
    margin-bottom: 50px;
  }

  .md-button {
    width: 130px;
    margin: 0 20px;
  }
}
/* SIXTH SECTION */
.sixth-section {
  margin: 50px auto;
  max-width: 1200px;
}
.cards-section {
  margin: 50px auto;
  max-width: 1200px;

  .md-card {
    margin: 10px auto;
    height: 280px;
  }

  .main-paragraph {
    max-width: 600px !important;
    margin: auto;
  }
}
.reviews-section {
  margin: 50px auto 100px auto;
  border: solid 1px black;
  height: 600px;

  .VueCarousel {
    width: 100%;
    min-height: 300px;
  }
}
.border {
  border: 1px solid #e5e5e5;
}
/* CARDS SECTION */
.cards-section {
  p,
  h2 {
    text-align: left;
  }
  .emp-cards {
    border-radius: 27px;
    position: relative;
    height: 280px;
    cursor: pointer;
    transition: 0.7s ease-in-out;
    transform-style: preserve-3d;

    &:hover {
      transform: rotateY(0.5turn);
    }
  }

  .background-image-card {
    position: absolute;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-position: center;
    background-size: cover;
    border-radius: 27px;
    transition: 1s ease-in-out;
    backface-visibility: hidden;
    &--back {
      transform: rotateY(0.5turn);
      width: 100%;
      border-radius: 27px;
      background-position: center;
      background-size: cover;
      height: 100%;
    }
  }
  .card-1 {
    background-image: url("../assets/img/empowering-agriculture-card-1.jpg");
  }
  .card-2 {
    background-image: url("../assets/img/empowering-agriculture-card-2.jpg");
  }
  .card-3 {
    background-image: url("../assets/img/empowering-agriculture-card-3.jpg");
  }
  .card-4 {
    background-image: url("../assets/img/empowering-agriculture-card-4.jpg");
  }
}

@media all and (min-width: 991px) {
  .btn-container {
    display: flex;
  }
}
@media all and (max-width: 960px) {
  .flex-no-wrap {
    flex-wrap: nowrap;
    flex-direction: row;
    padding-right: 0px;
    padding-left: 0px;
  }
  .flex-row-small {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    overflow-x: auto;
  }
}
</style>
