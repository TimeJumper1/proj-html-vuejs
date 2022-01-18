<template>
    <main>
        <Jumbotron/>
        <ServiceSection/>
        <CompanySection/>
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import ServiceSection from "./ServiceSection.vue";
import CompanySection from "./CompanySection.vue";

export default {
  name: "Main",
  components:{
      Jumbotron,
      ServiceSection,
      CompanySection
  }
};
</script>
    


<style scoped lang="scss">

</style>