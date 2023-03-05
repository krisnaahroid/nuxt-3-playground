<template>
  <div>
    <full-page ref="fullpage" :options="options" id="fullpage">
      <div class="section"><nuxt-img src="/logo.svg" /></div>
      <div class="section">Second section ...</div>
    </full-page>
  </div>
</template>

<script>
export default {
  data() {
    return {
      options: {
        licenseKey: "4LL6J-U37K9-8H097-2PSMK-VNYLP",
        sectionsColor: ["#41b883", "#ff5f45", "#0798ec"],
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.section {
  position: relative;
}

@media only screen and (min-device-width: 320px) and (max-device-width: 480px) and (-webkit-min-device-pixel-ratio: 2) {
  .fullpage {
    display: none !important;
  }

  .fullpage-m {
    display: block !important;
  }
}
</style>
