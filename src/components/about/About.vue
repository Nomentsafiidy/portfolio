<template>
  <div id="m_about">
    <transition name="fade" appear="fade" >
      <div class="m_about_left">
        <img src="./../../assets/img/nomentsafidy.png" alt="photo nomentsafidy" />
      </div>
    </transition>
    
    <transition name="translateX" appear="translateX" >
      <div class="m_about_right">
        <div class="m_about_title" >HI I'M <span class="name" >ANDRIAMIARANTSOA Nomentsafidy</span></div>
        <div class="m_about_subtitle">Fullstack javascript developer and Web Designer</div>
        <p>
          My name is ANDRIAMIARANTSOA Nomentsafidy. I am 24 years old. Lorem ipsum dolor sit amet, consectetur ascing elits, sed do eiusmod tempor incidunt ut labore et dolore mafgna aliqua. Ut enim ad mini vniam quis nerci, tation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis autes irure dolor in reprehenderit in etrs voluptate velit esse cillum dolore eu fugiat nulla pariatur. The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested.
          </p>
        <div class="m_about_social">
          <a href="#"><img src="./../../assets/svg/linkedin.svg" width="40" height="40" alt="linkedin"></a>
          <a href="#"><img src="./../../assets/svg/skype.svg" width="40" height="40" alt="skype"></a>
          <a href="#"><img src="./../../assets/svg/github.svg" width="40" height="40" alt="github"></a>
          <a href="#"><img src="./../../assets/svg/facebook.svg" width="40" height="40" alt="facebook"></a>
        </div>
        <button class="btn btn_danger mt_10" type="button">Download My Resume</button>
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" src="./about.scss"></style>
<style scoped >
  .fade-enter-active, .fade-leave-active {
    transition: opacity 2s;
  }
  .fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
    opacity: 0;
  }

  .translateX-enter-active, .translateX-leave-active {
    transition: transform 1.5s;
  }
  .translateX-enter, .translateX-leave-to /* .fade-leave-active below version 2.1.8 */ {
    transform: translateX(+200%);
  }
</style>
