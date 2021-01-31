<template>
  <div id="m_services" >
    <div class="m_title">
      Services
    </div>
    <div class="m_services_container">
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
      <ServiceItem class="m_item" />
    </div>
  </div>
</template>

<script>
import ServiceItem from "./components/ServiceItem"
export default {
  name: 'Services',
  components:{
    ServiceItem
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" src="./services.scss" ></style>
