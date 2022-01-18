<template>
  <section>
    <footer>
    <div class="container">
      <div class="footer-col">
        <h3>NEX GEN</h3>
        <p>A functional HTML Template for Corporate & Business</p>
        <h3> immagine e numero</h3>
        <h3> immagine e numero</h3>
        <h3> immagine e numero</h3>
        <h3>bottone</h3>
      </div>
      <div class="footer-col list">
        <!-- da popolare con un v-for -->
        <h3>NEX GEN</h3>
        <ul>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>

        </ul>
      </div>
      <div class="footer-col list">
        <!-- da popolare con un v-for -->
        <h3>NEX GEN</h3>
        <ul>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>

        </ul>
      </div>
      <div class="footer-col list">
        <!-- da popolare con un v-for -->
        <h3>NEX GEN</h3>
        <ul>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>
          <li>info</li>

        </ul>
      </div>
    </div>
    
  </footer>
  <div class="bottom-footer">
      <h4>Enjoy the low price. we are tracking any intention of piracy</h4>
      <h4>marchio copyright 2020 NEXGEN is Proudly Powered by Codings</h4>
      

    </div>
    <div class="up-click">
      immagine
    </div>
  </section>
        

</template>

<script>
export default {
  name: "Footer",
  props: {
    msg: String,
  },
};
</script>


<style scoped lang="scss">
section{
  background-color:#0d0d11 ;
  position: relative;
  footer{
    background-color:#111117 ;
    color: white;
  
    height: 500px;
    
    .container{
      width: 70%;
      height: 90%;
      margin: auto;
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      align-items: center;
      .footer-col{
        width: calc((100% / 4) - 10px);
        margin: 5px;
        padding: 7px;
      }
      .list{
        border-radius: 10px;
        background-color:#19191f ;
        ul{
          list-style-type:none;
        }
      }
    }
  
  }
  .bottom-footer{
    width: 70%;
    margin: auto;
    height: 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;
    
  }
  .up-click{
    position: absolute;
    right: 10px;
    bottom: 10px;
    color: white;
  }
}
</style>