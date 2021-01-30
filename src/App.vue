<template>
  <div id="app">
    <About />
    <Skill />
    <Education />
    <Services />
    <Portofolio />
    <Contact />
  </div>
</template>

<script>
import About from "./components/About";
import Skill from "./components/Skill"
import Education from "./components/Education"
import Services from "./components/Services"
import Portofolio from "./components/Portofolio"
import Contact from "./components/Contact"
export default {
  name: 'App',
  components: {
    About,
    Skill,
    Education,
    Services,
    Portofolio,
    Contact
  }
}
</script>

<style>
</style>
