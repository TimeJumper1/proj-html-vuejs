<template>
    <main>
        <Jumbotron/>
        <ServiceSection/>
    </main>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import ServiceSection from "./ServiceSection.vue";

export default {
  name: "Main",
  components:{
      Jumbotron,
      ServiceSection,
  }
};
</script>
    


<style scoped lang="scss">

</style>