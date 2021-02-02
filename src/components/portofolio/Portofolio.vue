<template>
  <div id="m_portofolio">
    <div class="m_title">
      Portofolio
    </div>
    <div class="m_container">
      <Work />
      <Work />
      <Work />
      <Work />
      <Work />
    </div>
  </div>
</template>

<script>
import Work from "./components/Work";
export default {
  name: "Portofolio",
  components: {
    Work,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" src="./portofolio.scss"></style>
