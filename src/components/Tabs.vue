<template>
  <md-card class="md-card-tabs" :class="[{ 'md-card-plain': plain }]">
    <md-card-header slot="header-title"> </md-card-header>

    <md-card-content class="md-layout main-content">
      <transition name="fade" mode="out-in">
        <div class="tab-content md-layout-item md-size-60 md-small-size-100">
          <div
            :class="getTabContent(index + 1)"
            v-for="(item, index) in tabName"
            :key="item"
            v-if="isActivePanel(tabName[index])"
          >
            <div class="md-layout-item">
              <div class="md-card info-card md-card-principal mx-2">
                <video playsinline autoplay muted loop>
                  <source :src="videoUrl" type="video/mp4" />
                </video>
                <md-card-content class="md-layout card-content">
                  <div
                    class="md-layout-item md-size-50 md-small-size-5 img-container"
                  >
                    <img
                      class="big-3-imgs"
                      :src="getImage(index)"
                      alt="Farmvi app mockup"
                    />
                  </div>
                  <div
                    class="md-layout-item text-padding md-size-50 md-small-size-90 text-white"
                  >
                    <slot :name="getTabContent(index + 1)">
                      This is the default text!
                    </slot>
                  </div>
                </md-card-content>
              </div>
            </div>
          </div>
        </div>
      </transition>
      <md-list class="nav-tabs md-layout-item md-size-40 md-small-size-100">
        <div class="three-stars"></div>
        <h2 class="text-green font-weight-bold big-3-title">Farmvi's Big 3</h2>
        <md-list-item
          v-for="(item, index) in tabName"
          @click="switchPanel(tabName[index])"
          :key="item"
        >
          <p
            class="numbers"
            :class="[
              { [getColorButton(colorButton)]: isActivePanel(tabName[index]) }
            ]"
          >
            {{ `0${index + 1}` }}
          </p>
          <p class="tab-names">{{ tabName[index] }}</p>
        </md-list-item>
      </md-list>
    </md-card-content>
  </md-card>
</template>

<script>
export default {
  props: {
    plain: Boolean,
    tabName: Array,
    tabIcon: Array,
    colorButton: {
      type: String,
      default: ""
    }
  },
  data() {
    return {
      activePanel: this.tabName[0],
      img1: require("@/assets/img/tab-pane-1-img.png"),
      img2: require("@/assets/img/tab-pane-2-img.png"),
      img3: require("@/assets/img/tab-pane-3-img.png"),
      videoUrl: require("@/assets/img/field-video.mp4")
    };
  },
  methods: {
    switchPanel(panel) {
      this.activePanel = panel;
    },
    isActivePanel(panel) {
      return this.activePanel == panel;
    },
    getColorButton: function(colorButton) {
      return "md-" + colorButton + "";
    },
    getTabContent: function(index) {
      return "tab-pane-" + index + "";
    },
    getImage(index) {
      switch (this.getTabContent(index + 1)) {
        case "tab-pane-1":
          return this.img1;
        case "tab-pane-2":
          return this.img2;
        case "tab-pane-3":
          return this.img3;
      }
    }
  }
};
</script>

<style lang="css">
video {
  position: absolute;
  top: 0;
  left: 0;
  object-fit: cover;
  height: 100% !important;
  width: 100%;
  border-radius: 27px;
}
.border {
  border: 1px solid #e5e5e5;
  border-radius: 5px;
  margin-bottom: 20px;
}
.text-green {
  color: #0a3939;
}
.text-white {
  color: #fff;
}
.font-weight-bold {
  font-weight: bold;
}
.tab-content {
  width: 500px;
}
.background-green {
  background-color: #0a3939;
  color: azure;
}
.pill-title {
  font-size: 32px;
  font-weight: 500;
  margin-bottom: 15px;
}
.pill-text {
  font-size: 18px;
  margin-bottom: 15px;
  margin-right: 30px;
}
.md-card {
  height: 100%;
}
@media screen and (max-width: 960px) {
  .main-content {
    flex-direction: column-reverse;
  }
}
.info-card {
  border-radius: 27px !important;
  background-image: url("../assets/img/big-3-background-2.jpg") !important;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  overflow: hidden;
}
.card-content {
  background: #00000096;
  position: relative;
  z-index: 2;
  margin: 0 !important;
  border-radius: 27px;
}
.nav-tabs {
  flex-flow: column !important;
  padding-left: 50px !important;
}
@media all and (max-width: 960px) {
  .nav-tabs {
    padding-left: 5px !important;
    padding-right: 5px !important;
  }
}
.three-stars {
  height: 50px;
  margin-bottom: 0px;
  background-image: url("../assets/img/three-stars-2.png");
  background-repeat: no-repeat;
}
@media all and (max-width: 960px) {
  .three-stars {
    background-position: center;
  }
  .big-3-title {
    text-align: center;
  }
}
.nav-items {
  display: block;
}
.md-list-item-content {
  justify-content: flex-start !important;
}

.md-list-item,
.md-list-item-button {
  height: 80px !important;
  border-radius: 0px !important;
  justify-content: flex-start !important;
}
.img-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
.big-3-imgs {
  max-width: 200px;
  max-height: 355px;
}

.md-yellow {
  color: #ff9a0386 !important;
}

.numbers {
  font-size: 4rem;
  font-weight: bold;
  color: #afafafa8;
  margin: 0px;
  position: absolute;
}

.tab-names {
  position: relative;
  text-transform: none;
  font-size: 20px;
  top: 22px;
  left: 20px;
  white-space: normal;
  color: #0a3939;
  font-weight: bold;
}
</style>
