<template>
    <full-page :options="options" id="fullpage" ref="fullpage">
        <!-- <div> -->
        <div class="section">
            <h3>vue-fullpage.js</h3>
        </div>
        <div class="section">
            <div class="slide">
                <h3>Slide 2.1</h3>
            </div>
            <div class="slide">
                <h3>Slide 2.2</h3>
            </div>
            <div class="slide">
                <h3>Slide 2.3</h3>
            </div>
        </div>
        <div class="section">
            <h3>Section 3</h3>
        </div>
        <!-- </div> -->
    </full-page>
</template>

<script>
// import { Fullpage } from "@/components/Fullpage";
    export default {
    data () {
      return {
        options: {
          licenseKey: 'YOUR_KEY_HERE',
          afterLoad: this.afterLoad,
          loopBottom: true,
          loopTop: true,
          loopHorizontal: true,
          scrollOverflow: true,
            // lazyLoading: true,
          scrollBar: false,
          menu: '#menu',
          navigation: true,
          anchors: ['page1', 'page2', 'page3'],
          sectionsColor: ['#41b883', '#ff5f45', '#0798ec', '#fec401', '#1bcee6', '#ee1a59', '#2c3e4f', '#ba5be9', '#b4b8ab']
        }
      }
    },
    }
</script>

<style lang="css" scoped>
  h3{
    text-align: center;
  }
</style>