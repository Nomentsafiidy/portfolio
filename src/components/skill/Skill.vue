<template>
  <div id="m_skill">
    <div class="m_title">
      Compétence
    </div>
    <div class="m_skill_content">
      <div class="m_skill_container">
        <div class="m_skill_title">Back End</div>
        <p>
          Divers langages et frameworks de programmation côté serveur
        </p>
        <div class="m_skill_items">
          <SkillItem :progress="80 * 1" title="Node Js" />
          <SkillItem :progress="75 * 1" title="Sails Js" />
          <SkillItem :progress="70 * 1" title="PHP" />
          <SkillItem :progress="65 * 1" title="Symfony" />
        </div>
      </div>
      <div class="m_skill_container">
        <div class="m_skill_title">Front End</div>
        <p>
          Divers langages et frameworks de programmation côté client
        </p>
        <div class="m_skill_items">
          <SkillItem :progress="75 * 1" title="Vue Js" />
          <SkillItem :progress="80 * 1" title="Angular" />
          <SkillItem :progress="85 * 1" title="Quasar" />
          <SkillItem :progress="80 * 1" title="Ionic" />
        </div>
      </div>
      <div class="m_skill_container">
        <div class="m_skill_title">Web Design</div>
        <p>
          Logiciel de création de modèles, de retouche et de création d'images
        </p>
        <div class="m_skill_items">
          <SkillItem :progress="85 * 1" title="Creative Design" />
          <SkillItem :progress="80 * 1" title="Figma" />
          <SkillItem :progress="90 * 1" title="Illustrator" />
          <SkillItem :progress="75 * 1" title="Photoshop" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SkillItem from "./components/Skillitem";
export default {
  name: "Skill",
  components: {
    SkillItem,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" src="./skill.scss"></style>
