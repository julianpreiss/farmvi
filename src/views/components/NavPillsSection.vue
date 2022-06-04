<template>
  <div class="wrapper">
    <div id="navigation-pills">
      <div class="md-layout">
        <div class="md-layout-item md-size-100">
          <tabs
            :tab-name="[
              'Hyperresolution Model',
              'Compare yourself with your neighbors',
              'Smart System Alarm'
            ]"
            plain
            nav-pills-icons
            color-button="yellow"
          >
            <!-- here you can add your content for tab-content -->
            <template slot="tab-pane-1">
              <h3 class="pill-title">Hyperresolution</h3>
              <p class="pill-text">
                Satellites stream large mapped areas at a near daily time
                interval. They also collect radition signals and bring
                high-resolution mapping images. However, this technology is
                still far from perfection in terms of resolution. Thus, our
                engineers developed customized algorithms so you can have the
                best in-field resolution as it is possible, providing you with
                analytics of your farmland.
              </p>
            </template>
            <template slot="tab-pane-2">
              <h3 class="pill-title">Compare yourself</h3>
              <p class="pill-text">
                Your farm is not alien to the macro-environment that surrounds
                it. Understanding how your neighbors perform, if there are
                anomalies or negative factors that affect all lands, is a
                crucial factor for the development of your crops.
              </p>
            </template>
            <template slot="tab-pane-3">
              <h3 class="pill-title">Smart Alarm</h3>
              <p class="pill-text">
                Using near-real time satellite images Farmvi can provide you
                early warning alerts of your crops. Timing and accuracy of
                anomalies are crucial to an effective monitoring.
              </p>
            </template>
          </tabs>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Tabs } from "@/components";

export default {
  components: {
    Tabs
  }
};
</script>

<style lang="css"></style>
