<template>
  <div id="m_header">
    <div class="m_logo">
      <a href="#">
        <span>Maizina.</span>
      </a>
    </div>
    <nav class="m_navigation">
      <a href="#aboutMe" @click.prevent="scrollTo('m_about')">Apropos</a>
      <a href="#skil" @click.prevent="scrollTo('m_skill')">Compétence</a>
      <a href="#services" @click.prevent="scrollTo('m_services')">Services</a>
      <a href="#portofolio" @click.prevent="scrollTo('m_portofolio')"
        >Portofolio</a
      >
      <a href="#education" @click.prevent="scrollTo('m_education')"
        >Education</a
      >
      <a href="#contact" @click.prevent="scrollTo('m_contact')">Contact</a>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
  methods: {
    scrollTo(elementId) {
      let el = document.querySelector(`#${elementId}`);
      el.scrollIntoView({
        behavior: "smooth",
        block: "start",
      });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style src="./header.scss" lang="scss"></style>
