<template>
  <div id="app">
    <Header />
    <About />
    <Skill />
    <Services />
    <Portofolio />
    <Education />
    <Contact />
  </div>
</template>

<script>
import Header from "./components/header/Header";
import About from "./components/about/About";
import Skill from "./components/skill/Skill";
import Education from "./components/education/Education";
import Services from "./components/services/Services";
import Portofolio from "./components/portofolio/Portofolio";
import Contact from "./components/contact/Contact";
export default {
  name: "App",
  components: {
    Header,
    About,
    Skill,
    Education,
    Services,
    Portofolio,
    Contact,
  },
};
</script>

<style lang="scss">
@import url("./assets/scss/maizina.scss");
#app {
  height: 100%;
}
</style>
