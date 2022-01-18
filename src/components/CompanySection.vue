<template>
  <section>
    <div class="col sinistra">
      <div class="top-info">
        <h4>ABOUT THE NETWORK</h4>
        <h2>The Company</h2>
        <p>for 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients</p>
      </div>
      <div class="info-container">
        <!-- si potra usare un v-for? -->
        <div class="info-card">

        </div>
        <div class="info-card">

        </div>
        <div class="info-card">

        </div>
        <div class="info-card">

        </div>
      </div>
      <div>
        <span class="btn">bottone</span><span class="btn">bottone</span>
      </div>
    </div>
    <div class="col destra">
      <img class="image" src="../assets/img/about-4.jpg" alt="about img">
    </div>
    <div class="bullets-decorations top">
      <img src="../assets/img/bullets.png" alt="decorazioni">
    </div>
    <div class="bullets-decorations bottom">
      <img src="../assets/img/bullets.png" alt="decorazioni">
    </div>
  </section>
         
</template>

<script>
export default {
  name: "CompanySection",
  
};
</script>


<style scoped lang="scss">
section{
  display: flex;
  height:700px ;
  position: relative;
  
  // test
  color: white;
  background-color: black;
  .col{
    width: 50%;
    .image{
      width: 100%;
      max-height: 100%;
    }
    .info-container{
      display: flex;
      flex-wrap: wrap;
      flex-direction: row;
      .info-card{
        width: calc((100% / 2) - 20px);
        margin: 10px;
        // test
        background-color: pink;
        height: 150px;
      }
    }
  }
  .sinistra{
    padding: 70px 20px 70px 250px ;
  }
  .bullets-decorations{
    width: 170px;
    height: 70px;
    overflow: hidden;
    position: absolute;
    img{
      width: 100%;
      overflow: hidden;
      opacity: 0.5;
    }
  }
  .top{
    transform: translate(-50% , 0);
    top: -35px;
    left: 50%;
  }
  .bullets-decorations{
    transform: translate(-50% , 0);
    bottom: -35px;
    left: 50%;
  }
}
</style>