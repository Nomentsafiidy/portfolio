<template>
  <section class="m_service_item">
        <img
          class="m_service_img"
          src="./../../../assets/logo.png"
          alt="Vue Js"
        />
        <h6 class="m_service_item_title">LOREM ISPUM</h6>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Est delectus
          rerum distinctio molestiae accusamus reprehenderit praesentium
        </p>
    </section>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped >
  .m_service_item{
    margin: 0 15px;
    padding: 20px;
    text-align: center;
    width: 250px;
    font-size: 18px;
    font-family: "Raleway-Bold";
    color: #333333;
    .m_service_img{
      height: 100px;
      width: auto;
    }
    .m_service_item_title{
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