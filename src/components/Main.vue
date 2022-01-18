<template>
    <main>
        <Jumbotron/>
        <ServiceSection/>
        <CompanySection/>
        <ActionSection/>
        <NumbersSection/>
        <FormSection/>
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import ServiceSection from "./ServiceSection.vue";
import CompanySection from "./CompanySection.vue";
import ActionSection from "./ActionSection.vue";
import NumbersSection from "./NumbersSection.vue";
import FormSection from "./FormSection.vue";

export default {
  name: "Main",
  components:{
      Jumbotron,
      ServiceSection,
      CompanySection,
      ActionSection,
      NumbersSection,
      FormSection
  }
};
</script>
    


<style scoped lang="scss">

</style>