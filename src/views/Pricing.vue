<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout animate__animated animate__fadeInDown">
          <div class="md-layout-item text-center md-size-100">
            <h1 class="title">Pricing</h1>
            <h4>
              We have different plans for you to try.
            </h4>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section">
        <div class="container">
          <div class="md-layout">
            <div
              class="md-layout-item md-size-66 md-xsmall-size-100 mx-auto text-center"
            >
              <h2 class="title text-center green-text">Our Plans</h2>
            </div>
          </div>
          <div class="md-layout">
            <div class="md-layout-item md-size-33 md-small-size-100 p-relative">
              <div class="card-container p-relative">
                <md-card
                  class="plan-card p-absolute c-back card-background-1"
                ></md-card>
                <md-card class="plan-card">
                  <div class="three-stars background-center"></div>
                  <md-card-content>
                    <div class="text-center">
                      <h3 class="font-weight-bold">Free Plan</h3>
                      <p>0€ ha/€ /mo</p>
                    </div>
                    <ul>
                      <li>Historical data and daily prescription maps</li>
                      <li>Alarm system, weather forecast</li>
                      <li>Task manager, audio notes, cost calculator</li>
                      <li>Posturage module</li>
                    </ul>
                    <div class="text-center">
                      <md-button class="md-round white-transparent-button">
                        Get Started
                      </md-button>
                    </div>
                  </md-card-content>
                </md-card>
              </div>
            </div>
            <div class="md-layout-item md-size-33 md-small-size-100 p-relative">
              <div class="card-container p-relative">
                <md-card
                  class="plan-card p-absolute c-back card-background-2"
                ></md-card>
                <md-card class="plan-card">
                  <div class="three-stars background-center"></div>
                  <md-card-content>
                    <div class="text-center">
                      <h3 class="font-weight-bold">Basic Plan</h3>
                      <p>0€ ha/€ /mo</p>
                    </div>
                    <ul>
                      <li>Historical data and daily prescription maps</li>
                      <li>Alarm system, weather forecast</li>
                      <li>Task manager, audio notes, cost calculator</li>
                      <li>Posturage module</li>
                    </ul>
                    <div class="text-center">
                      <md-button class="md-round white-transparent-button">
                        Get Started
                      </md-button>
                    </div>
                  </md-card-content>
                </md-card>
              </div>
            </div>
            <div class="md-layout-item md-size-33 md-small-size-100 p-relative">
              <div class="card-container p-relative">
                <md-card
                  class="plan-card p-absolute c-back card-background-3"
                ></md-card>
                <md-card class="plan-card premium-plan">
                  <div class="three-stars background-center"></div>
                  <md-card-content>
                    <div class="text-center">
                      <h3 class="font-weight-bold">Premium Plan</h3>
                      <p>0€ ha/€ /mo</p>
                    </div>
                    <ul>
                      <li>Historical data and daily prescription maps</li>
                      <li>Alarm system, weather forecast</li>
                      <li>Task manager, audio notes, cost calculator</li>
                      <li>Posturage module</li>
                    </ul>
                    <div class="text-center">
                      <md-button class="md-round white-transparent-button">
                        Get Started
                      </md-button>
                    </div>
                  </md-card-content>
                </md-card>
              </div>
            </div>
          </div>
        </div>
        <div class="container">
          <div class="md-layout contact-section align-center">
            <h2 class="text-green font-weight-bold">
              Do you want a custom plan that fit your necessities? Get in touch
              with us
            </h2>
            <md-button class="md-round green-transparent-button">
              Get Started
            </md-button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  bodyClass: "landing-page",
  props: {
    header: {
      type: String,
      default: require("@/assets/img/header-image.jpg")
    }
  },
  data() {
    return {
      name: null,
      email: null,
      message: null,
      roadmap1: require("@/assets/img/roadmap-1.png"),
      roadmap2: require("@/assets/img/roadmap-2.png")
    };
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
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
.font-weight-bold {
  font-weight: bold;
}
.font-weight-semibold {
  font-weight: 500;
}
.green-text {
  color: #0a3939;
}
.orange-text {
  color: #ff9c03;
}
.white-text {
  color: #fff !important;
}
.align-left {
  text-align: left;
}
.align-center {
  text-align: center;
  justify-content: center;
}
.background-center {
  background-position: center;
  background-image: url("../assets/img/three-stars-2.png");
  background-size: contain;
  height: 40px;
}
.md-button {
  max-width: 110px;
  align-self: center;
}
.rounded-border {
  border-radius: 27px;
}
.white-transparent-button {
  background-color: transparent !important;
  border: solid 1px white;
}
.white-transparent-button:hover {
  background-color: white !important;
  border: solid 1px white;
  color: #0a3939 !important;
}
.green-transparent-button {
  background-color: transparent !important;
  border: solid 1px #0a3939;
  color: #0a3939 !important;
}
.green-transparent-button:hover {
  background-color: #0a3939 !important;
  border: solid 1px #0a3939;
  color: white !important;
}
.page-header {
  height: 80vh;
}
.plan-card {
  background-color: #0a3939 !important;
  color: white !important;
  height: 450px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 95%;
  margin: 0 auto;
}
.p-relative {
  position: relative;
  margin: 10px auto;
}
.p-absolute {
  position: absolute;
  top: 15px;
  right: 0px;
  width: 88%;
}
@media all and (max-width: 960px) {
  .plan-card {
    width: 100%;
    margin: 0 auto;
    padding: 0;
    width: 300px;
  }
  .p-absolute {
    right: 25px;
  }
  .card-container {
    width: 400px;
  }
}
@media all and (max-width: 500px) {
  .p-absolute {
    right: -10px;
  }
  .card-container {
    width: 270px;
  }
  .plan-card {
    padding: 0;
    width: 270px;
  }
}
.premium-plan {
  background-color: #c25721 !important;
  color: white !important;
}
.c-back {
  background-position: center;
  background-size: cover;
}
.card-background-1 {
  background-image: url("../assets/img/pricing-1.jpg");
}
.card-background-2 {
  background-image: url("../assets/img/pricing-2.jpg");
}
.card-background-3 {
  background-image: url("../assets/img/pricing-3.jpg");
}
.contact-section {
  max-width: 80%;
  align-self: center;

  h2 {
    font-size: 2rem;
    text-align: center;
  }
}
.md-has-textarea + .md-layout {
  margin-top: 15px;
}
</style>
