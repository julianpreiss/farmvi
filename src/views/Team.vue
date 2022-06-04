<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout animate__animated animate__fadeInDown">
          <div class="md-layout-item md-size-100 text-center">
            <h1 class="title">ABOUT US</h1>
            <h4>
              Meet the Farmvi team and our values.
            </h4>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised rounded-border">
      <div class="section">
        <div class="container">
          <div class="md-layout">
            <div
              class="md-layout-item md-size-66 md-xsmall-size-100 mx-auto text-center"
            >
              <h2 class="title text-center green-text">Our team</h2>
              <h3 class="description">
                Meet the brains behind farmvi
              </h3>
            </div>
          </div>
          <div class="team-section text-center">
            <div class="md-layout flex">
              <div
                class="md-layout-item images-section md-size-66 md-small-size-100"
              >
                <div class="md-layout big-images">
                  <div class="md-layout-item md-size-33 md-xsmall-size-100">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg1"
                          alt="Sebastian Palacio"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Sebastián Palacio</h4>
                          <p>
                            CEO/Co-founder
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-33 md-xsmall-size-100">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg2"
                          alt="Ignacio Lopez"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Ignacio Lopez</h4>
                          <p>
                            AI Leader / Co-founder
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-33 md-xsmall-size-100">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg3"
                          alt="Pouria Ruhi"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Pouria Ruhi</h4>
                          <p>
                            Business dev leader/Co-founder
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                </div>
                <div class="md-layout small-images">
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg6"
                          alt="Diego Cataldi"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Diego Cataldi</h4>
                          <p>
                            Project Manager
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg5"
                          alt="Cecilia Justo"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Cecilia Justo</h4>
                          <p>
                            Agriculture Engineer
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg4"
                          alt="Julian Preiss"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Julian Preiss</h4>
                          <p>
                            Web Developer
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg7"
                          alt="Convoi"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Convoi</h4>
                          <p>
                            Branding
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                </div>
                <div class="md-layout small-images">
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg8"
                          alt="Athene group"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Athene group</h4>
                          <p>
                            Accountability
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg9"
                          alt="Emanuel Frene"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Emanuel Frene</h4>
                          <p>
                            Accountant
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg10"
                          alt="Federico Lozada"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Federico Lozada</h4>
                          <p>
                            Lead Developer
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg11"
                          alt="Gerardo Sepúlveda"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Gerardo Sepúlveda</h4>
                          <p>
                            UX/UI designer
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                </div>
                <div class="md-layout small-images">
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg12"
                          alt="Pablo Lopez"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>Pablo Lopez</h4>
                          <p>
                            Fullstack Developer Jr
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                  <div class="md-layout-item md-size-25 md-xsmall-size-50">
                    <div class="md-card rounded-border">
                      <md-card-content class="padding-0">
                        <img
                          class="img-responsive"
                          :src="teamImg13"
                          alt="John Molloy"
                        />
                        <div class="p-absolute text-white align-right">
                          <h4>John Molloy</h4>
                          <p>
                            Strategic Developer
                          </p>
                        </div>
                      </md-card-content>
                    </div>
                  </div>
                </div>
              </div>
              <div class="md-layout-item md-size-33 md-small-size-100">
                <div class="info">
                  <h3 class="info-title green-text">Team Overview</h3>
                  <p>
                    We are a fast-growing small team of xx interdisciplinary
                    members who are passionate about agriculture. We believe
                    that the core strenght of our unique product is based on the
                    combination of high-level skilled people who are part of
                    this amazing adventure: Agriculture engineers, software
                    engineers, artificial intelligence developers, UX designers,
                    strategy developers, etc. Everyone contributing to make the
                    life of farmers easier.
                  </p>
                  <h3 class="info-title green-text">Team Stadistics</h3>
                  <div class="number-pills">
                    <div class="pill">
                      <div class="number orange-text">18</div>
                      <div>People</div>
                    </div>
                    <div class="pill">
                      <div class="number orange-text">7</div>
                      <div>Countries</div>
                    </div>
                    <div class="pill">
                      <div class="number orange-text">0</div>
                      <div>Offices</div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="mission-section text-center">
        <div class="container">
          <md-card class="flex info-card rounded-border">
            <div
              class="md-layout-item md-size-60 md-small-size-100 green-background"
            >
              <md-card-content>
                <h2 class="orange-text font-weight-bold">
                  /F&#60;rmvi's mission_
                </h2>
                <p class="md-subheading white-text">
                  Make the life of farmers easier
                </p>
                <div class="align-left text-section white-text">
                  <p>
                    When you are in farming, the weather is on your mind all the
                    time. A late spring freeze, an extended midsummer dry can
                    easily make you lose the entire crop year.
                  </p>
                  <p>
                    Crops are the result of a complex mixing between conditions
                    and human decision.
                  </p>
                  <p>
                    Farmers don't take a break, they are moved by the compass of
                    the wind, they trust in the sun and the rain. They use
                    intuitive knowledge to work, but most of the time best
                    predictive abilities have wide margins of error.
                  </p>
                  <p>
                    Farmvi was born to make farmers life easier. Like a north
                    star that served as a reliable beacon guide, is the mentor
                    to farmers across the crop cycle.
                  </p>
                </div>
              </md-card-content>
            </div>
            <div
              class="md-layout-item md-size-40 md-small-size-100 mockup-background"
            >
              <md-card-content></md-card-content>
            </div>
          </md-card>
        </div>
      </div>
      <div class="section roadmap-section">
        <div class="container">
          <div class="md-layout">
            <div class="md-layout-item md-size-66 md-xsmall-size-100 mx-auto">
              <h2 class="text-center title">Farmvi's Roadmap</h2>
              <p class="text-center md-subheading">
                What we did in the past and what are our next goals
              </p>
            </div>
          </div>
          <div class="md-layout">
            <vue-glide :autoplay="5000" :perView="slidesPerView">
              <vue-glide-slide>
                <div class="md-layout-item">
                  <span class="year-grey">2019</span>
                  <img
                    class="roadmap-imgs"
                    :src="roadmap1"
                    alt="Goat Detector"
                  />
                  <h3 class="font-weight-bold text-green">Goat detector</h3>
                  <p>
                    Farmvi is the result of a particular story between a
                    veterinarian and the problems he had to find his goats in
                    the mountains. Everything started in 2019 with a drone that
                    was capable of detecting lost goats.
                  </p>
                </div>
              </vue-glide-slide>
              <vue-glide-slide>
                <div class="md-layout-item">
                  <span class="year-grey">2020</span>
                  <img
                    class="roadmap-imgs"
                    :src="roadmap2"
                    alt="Charge Program"
                  />
                  <h3 class="font-weight-bold text-green">Charge program</h3>
                  <p>
                    In 2020 we were accepted to the incubator Charge program,
                    where we pivoted thousand of times before we reach to the
                    final idea of combining satellite images, computer vision
                    and agriculture.
                  </p>
                </div>
              </vue-glide-slide>
              <vue-glide-slide>
                <div class="md-layout-item">
                  <span class="year-grey">2021</span>
                  <img
                    class="roadmap-imgs"
                    :src="roadmap3"
                    alt="Charge Program"
                  />
                  <h3 class="font-weight-bold text-green">First MVP</h3>
                  <p>
                    During the summer of 2021, we tested for the first time our
                    MVP with several farmers in Norway.
                  </p>
                </div>
              </vue-glide-slide>
              <vue-glide-slide>
                <div class="md-layout-item">
                  <span class="year-grey">2021</span>
                  <img
                    class="roadmap-imgs"
                    :src="roadmap4"
                    alt="Goat Detector"
                  />
                  <h3 class="font-weight-bold text-green">
                    First-round-investment
                  </h3>
                  <p>
                    Farmvi is the result of a particular story between a
                    veterinarian and the problems he had to find his goats in
                    the mountains. Everything started in 2019 with a drone that
                    was capable of detecting lost goats.
                  </p>
                </div>
              </vue-glide-slide>
              <vue-glide-slide>
                <div class="md-layout-item">
                  <span class="year-grey">2022</span>
                  <img
                    class="roadmap-imgs"
                    :src="roadmap5"
                    alt="Charge Program"
                  />
                  <h3 class="font-weight-bold text-green">Charge program</h3>
                  <p>
                    In 2020 we were accepted to the incubator Charge program,
                    where we pivoted thousand of times before we reach to the
                    final idea of combining satellite images, computer vision
                    and agriculture.
                  </p>
                </div>
              </vue-glide-slide>
            </vue-glide>
          </div>
        </div>
      </div>
      <div class="section values-section">
        <div class="md-layout-item md-size-100">
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
      </div>
    </div>
  </div>
</template>

<script>
import { Glide, GlideSlide } from "vue-glide-js";
import "vue-glide-js/dist/vue-glide.css";
export default {
  bodyClass: "landing-page",
  components: {
    [Glide.name]: Glide,
    [GlideSlide.name]: GlideSlide
  },
  props: {
    header: {
      type: String,
      default: require("@/assets/img/header-image.jpg")
    },
    teamImg1: {
      type: String,
      default: require("@/assets/img/team/sebastian-palacio.jpg")
    },
    teamImg2: {
      type: String,
      default: require("@/assets/img/team/ignacio-lopez.jpg")
    },
    teamImg3: {
      type: String,
      default: require("@/assets/img/team/pouria.jpg")
    },
    teamImg4: {
      type: String,
      default: require("@/assets/img/team/julian-preiss.jpg")
    },
    teamImg5: {
      type: String,
      default: require("@/assets/img/team/cecilia-justo.jpg")
    },
    teamImg6: {
      type: String,
      default: require("@/assets/img/team/diego-cataldi.jpg")
    },
    teamImg7: {
      type: String,
      default: require("@/assets/img/team/convoi.jpg")
    },
    teamImg8: {
      type: String,
      default: require("@/assets/img/team/athene-group.jpg")
    },
    teamImg9: {
      type: String,
      default: require("@/assets/img/team/emanuel-frene.jpg")
    },
    teamImg10: {
      type: String,
      default: require("@/assets/img/team/federico-lozada.jpg")
    },
    teamImg11: {
      type: String,
      default: require("@/assets/img/team/gerardo-sepulveda.jpg")
    },
    teamImg12: {
      type: String,
      default: require("@/assets/img/team/pablo-lopez.jpg")
    },
    teamImg13: {
      type: String,
      default: require("@/assets/img/team/john-molloy.jpg")
    }
  },
  data() {
    return {
      name: null,
      email: null,
      message: null,
      roadmap1: require("@/assets/img/roadmap-1.png"),
      roadmap2: require("@/assets/img/roadmap-2.png"),
      roadmap3: require("@/assets/img/roadmap-3.png"),
      roadmap4: require("@/assets/img/roadmap-4.png"),
      roadmap5: require("@/assets/img/roadmap-5.png")
    };
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    },
    slidesPerView() {
      return window.innerWidth > 800 ? 2 : 1;
    }
  }
};
</script>

<style lang="scss" scoped>
.border {
  border: 1px solid black;
}
.flex {
  display: flex;
}
@media screen and (max-width: 968px) {
  .flex {
    flex-direction: column-reverse;
  }
}
.font-weight-bold {
  font-weight: bold;
}
.font-weight-semibold {
  font-weight: 500;
}
.green-background {
  background-color: #0a3939;
}
.green-text {
  color: #0a3939 !important;
}
.orange-text {
  color: #ff9c03;
}
.white-text {
  color: #fff;
}
.align-left {
  text-align: left;
}
.align-right {
  text-align: right;
}
.responsive {
  width: 100%;
  height: auto;
}
.rounded-border {
  border-radius: 27px;
  overflow: hidden;
}
.padding-0 {
  padding: 0 !important;
}
.margin-0 {
  margin: 0 !important;
}
.page-header {
  height: 80vh;
}
.team-section {
  .images-section {
    .big-images {
      margin-top: 0;
      .md-card {
        height: 95%;
        margin: 0;

        .img-responsive {
          width: 100%;
          height: 100%;
        }
        .p-absolute {
          max-width: 60%;
        }
        h4 {
          margin-bottom: 5px;
          font-weight: 500;
          font-size: 1.5rem;
        }

        p {
          margin-top: 0;
          font-size: 1rem;
        }
      }
    }
    .small-images {
      .md-card {
        margin: 0;
        height: 95%;
      }
      .p-absolute {
        max-width: 80%;
      }
      h4 {
        margin-bottom: 0px;
        font-weight: 500;
        font-size: 1.2rem;
      }

      p {
        margin-top: 0;
        font-size: 0.9rem;
      }
    }
    // @media all and (min-width: 960px) {
    .img-responsive {
      transition: 0.3s ease-in-out;
    }
    .p-absolute:hover ~ .img-responsive,
    .img-responsive:hover {
      opacity: 0.6;
      transform: scale(1.05);
    }

    .p-absolute {
      transition: opacity 0.5s ease-out;
      opacity: 0;
    }

    .padding-0 {
      background: black;
    }

    .img-responsive:hover ~ .p-absolute,
    .p-absolute:hover {
      display: block;
      opacity: 1;
    }
    // }
    .p-absolute {
      position: absolute;
      bottom: 15px;
      right: 15px;
    }
  }
  .info {
    text-align: left;
    padding-top: 0px;

    .info-title {
      font-size: 32px;
      font-weight: bold;
      margin-top: 0px;
    }

    .number-pills {
      .pill {
        display: inline-block;
        width: 70px;
        margin-right: 16px;

        .number {
          font-size: 40px;
          font-weight: bold;
          margin-bottom: 7px;
        }
      }
    }
  }
}
.mission-section {
  margin: auto;
  max-width: 1366px;
  .info-card {
    margin: 0;
    height: 100%;

    .md-card-content {
      margin-bottom: 25px;
    }
  }
  .mockup-background {
    background-image: url("../assets/img/background-farmvi-team.jpg");
    background-size: 150%;
    animation: AnimateBG 15s ease-in-out infinite;
  }
  @keyframes AnimateBG {
    0% {
      background-position: 40% 80%;
    }
    25% {
      background-position: 40% 40%;
    }
    50% {
      background-position: 100% 50%;
    }
    75% {
      background-position: 100% 80%;
    }
    100% {
      background-position: 40% 80%;
    }
  }
  .text-section {
    margin-top: 20px;
  }
}
.roadmap-section {
  margin: auto;
  max-width: 1366px;
  .year-grey {
    color: #e4e4e4;
    font-size: 3rem;
    font-weight: 800;
    padding-bottom: 20px;
    display: block;
  }
  .glide__slide {
    height: 100%;
    padding-top: 15px;
  }
  .roadmap-imgs {
    max-height: 280px;
  }
}
.values-section {
  margin: auto;
  max-width: 1366px;
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
.md-card-actions.text-center {
  display: flex;
  justify-content: center !important;
}
.contact-form {
  margin-top: 30px;
}

.md-has-textarea + .md-layout {
  margin-top: 15px;
}
</style>
