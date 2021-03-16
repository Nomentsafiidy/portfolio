<template>
  <section class="m_service_item">
    <span class="material-icons m_service_img">
      {{ iconName }}
    </span>
    <h2 class="m_service_item_title">{{ title }}</h2>
    <p>
      {{ description }}
    </p>
  </section>
</template>

<script>
export default {
  name: "SeviceItem",
  props: {
    title: {
      type: String,
    },
    description: {
      type: String,
    },
    iconName: {
      type: String,
    },
  },
};
</script>

<style lang="scss" scoped>
.m_service_item {
  margin: 0 15px;
  padding: 20px;
  text-align: center;
  width: 250px;
  font-size: 18px;
  font-family: "Raleway-Bold";
  color: #333333;
  .m_service_img {
    font-size: 100px;
  }
  .m_service_item_title {
    margin: 15px 0px;
  }
  p {
    margin: 10px 0px;
    font-size: 13px;
    line-height: 24px;
    color: #666666;
    font-family: "Raleway-Medium";
  }
}
</style>
