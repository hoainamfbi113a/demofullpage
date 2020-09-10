<template>
  <div>
    <full-page ref="fullpage" :options="options">
      <div class="section">
        <button class="next" @click="$refs.fullpage.api.moveSectionDown()">Next</button>
        Section 1
      </div>
      <div class="section">
        <button class="prev" @click="$refs.fullpage.api.moveSectionUp()">Prev</button>
        Section 2
      </div>
    </full-page>
  </div>
</template>

<script>
    export default {
        data() {
        return {
          options: {
            afterLoad: this.afterLoad,
            licenseKey: 'YOUR_KEY_HERE',
            controlArrows: true,
            scrollBar: true
          }
        }
      },

      methods: {
        afterLoad() {
          console.log("Emitted 'after load' event.");
        }
      }
    }
</script>

<style lang="scss" scoped>

</style>