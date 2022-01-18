<template>
    <main>
        <Jumbotron/>
        <ServiceSection/>
        <CompanySection/>
        <ActionSection/>
        <NumbersSection/>
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import ServiceSection from "./ServiceSection.vue";
import CompanySection from "./CompanySection.vue";
import ActionSection from "./ActionSection.vue";
import NumbersSection from "./NumbersSection.vue";

export default {
  name: "Main",
  components:{
      Jumbotron,
      ServiceSection,
      CompanySection,
      ActionSection,
      NumbersSection
  }
};
</script>
    


<style scoped lang="scss">

</style>