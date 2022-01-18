<template>
    <main>
        <Jumbotron/>
        <ServiceSection/>
        <CompanySection/>
        <ActionSection/>
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import ServiceSection from "./ServiceSection.vue";
import CompanySection from "./CompanySection.vue";
import ActionSection from "./ActionSection.vue";

export default {
  name: "Main",
  components:{
      Jumbotron,
      ServiceSection,
      CompanySection,
      ActionSection
  }
};
</script>
    


<style scoped lang="scss">

</style>