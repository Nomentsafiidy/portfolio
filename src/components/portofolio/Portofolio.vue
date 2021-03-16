<template>
  <div id="m_portofolio">
    <div class="m_title">
      Portofolio
    </div>
    <div class="m_container">
      <Work v-for="(work, i) in works" :key="i" :work="work" />
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
  data: () => {
    return {
      works: [
        {
          title: "Mon portofolio",
          category: " dev : web",
          imgUrl: "portofolio.png",
        },
        {
          title: "Boook",
          category: " dev : web / mobile",
          imgUrl: "boook.png",
        },
        {
          title: "Kewee",
          category: "dev : web / mobile",
          imgUrl: "work.jpg",
        },
        {
          title: "Integration d'un site",
          category: "dev : web / mobile",
          imgUrl: "work.jpg",
        },
        {
          title: "Koba",
          category: " Desktop / web / mobile",
          imgUrl: "koba.png",
        },
        {
          title: "Akata",
          category: " création du Logo ",
          imgUrl: "akata.png",
        },
        {
          title: "Goavana",
          category: " création du Logo ",
          imgUrl: "goavana.png",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" src="./portofolio.scss"></style>
