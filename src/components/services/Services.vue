<template>
  <div id="m_services">
    <div class="m_title">
      Services
    </div>
    <div class="m_services_container">
      <ServiceItem
        class="m_item"
        v-for="(service, index) in services"
        :key="index"
        :description="service.description"
        :title="service.title"
        :iconName="service.iconName"
      />
    </div>
  </div>
</template>

<script>
import ServiceItem from "./components/ServiceItem";
export default {
  name: "Services",
  components: {
    ServiceItem,
  },
  data: () => {
    return {
      services: [
        {
          title: "Développements spécifiques",
          description:
            "Des outils adaptés à votre coeur de métier, applications & solutions personnalisées",
          iconName: "important_devices",
        },
        {
          title: "Intergration web",
          description:
            "Des intergrations (x)HTML / css respectueuses des standards du web",
          iconName: "devices_other",
        },
        {
          title: "Conception grafique & webdesign",
          description:
            "Logos, templates web, plaquettes publicitaires, cartes de visite, newsletters...",
          iconName: "design_services",
        },
        {
          title: "Dynamisme des pages",
          description:
            "Des animations de contenu non intrusives pour embellir votre projet",
          iconName: "animation",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" src="./services.scss"></style>
