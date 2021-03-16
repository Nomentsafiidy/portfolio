<template>
  <div class="m_work_item">
    <div class="img">
      <div class="filter"></div>
      <img :src="require(`@/assets/img/${work.imgUrl}`)" alt="work" />
    </div>
    <div class="m_work_description">
      <div class="m_title">{{ work.title }}</div>
      <div class="m_category">{{ work.category }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Work",
  props: {
    work: {
      type: Object,
    },
  },
};
</script>

<style lang="scss" scoped>
.m_work_item {
  width: 312px;
  background: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  margin: 15px;
  &:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
    .img {
      .filter {
        width: 100%;
        height: 100%;
      }
    }
    .m_work_description {
      background: var(--warning-color);
      .m_title {
        color: white;
      }
      .m_category {
        color: white;
      }
    }
  }
  .img {
    height: 312px;
    width: 312px;
    position: relative;
    img {
      z-index: 1;
      height: 100%;
      width: 100%;
      object-fit: cover;
    }
    .filter {
      background: rgba(black, 0.5);
      position: absolute;
      width: 0px;
      height: 100%;
      z-index: 2;
      transition: width 0.8s;
    }
  }
  .m_work_description {
    text-align: center;
    font-family: "Raleway-Bold";
    padding: 10px;
    transition: background-color 0.7s;
    .m_title {
      font-size: 16px;
      color: #333333;
      margin: 0;
      transition: color 0.4s;
    }
    .m_category {
      font-size: 14px;
      color: #666666;
      margin-bottom: 5px;
      transition: color 0.4s;
    }
  }
}
</style>
