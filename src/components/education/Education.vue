<template>
  <div id="m_education">
    <div class="m_title">Education</div>
    <div class="m_education_container">
      <div v-for="(item, index) in items" :key="index" class="m_education_item">
        <div class="m_period">{{ item.period }}</div>
        <div class="m_cursus">{{ item.cursus }}</div>
        <div class="m_school">{{ item.school }}</div>
        <p class="m_description">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Education",
  data: () => {
    return {
      items: [
        {
          period: "2020-2021",
          cursus: "Etude Supérieur",
          school: "ENI Fianarantsoa",
          description:
            "deuxième année de formation en Master. Diplôme de Master II en informatique option : Génie logiciel et base de données",
        },
        {
          period: "2018-2019",
          cursus: "Etude Supérieur",
          school: "ENI Fianarantsoa",
          description:
            "Troisième année de formation en Licence Professionnelle. Diplôme de licence Professionnelle en informatique Option : Génie logiciel et base de données",
        },
        {
          period: "2014-2015",
          cursus: "Etude Secondaire",
          school: "Lycée Jules Ferry Faravohitra (LJF)",
          description:
            "Terminale scientifique.	Diplôme :	BAC Série C session Août 2015",
        },
        {
          period: "2013-2014",
          cursus: "Etude Secondaire",
          school: "Lycée Jules Ferry Faravohitra (LJF)",
          description:
            "Terminale litéraire.	Diplôme :	BAC Série A2 session Août 2014",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style src="./education.scss" lang="scss"></style>
