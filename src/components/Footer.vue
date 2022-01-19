<template>
  <section>
    <footer>
    <div class="container">
      <div class="footer-col">
        <h3 class="logo"><span class="decor">NEX</span>GEN</h3>
        <p>A functional HTML Template for Corporate & Business</p>
        <h4><span><i class="fas fa-phone-alt"></i></span> +1 (305) 1234-5678</h4>
        <h4><span><i class="fas fa-envelope"></i></span>hello@example.com</h4>
        <h4><span><i class="fas fa-map-marker-alt"></i></span>Main Avenue, 987</h4>
        <span class="btn">GET IN TOUCH</span>
      </div>
      <div v-for="(footerItem, index) in footerInfo" :key="index" class="footer-col list">
        <!-- da popolare con un v-for -->
        <h3>{{footerItem.title}}</h3>
        <h5><i class="fas fa-chevron-right"></i>{{footerItem.firstListElement}}</h5>
        <h5><i class="fas fa-chevron-right"></i>{{footerItem.secondListElement}}</h5>
        <h5><i class="fas fa-chevron-right"></i>{{footerItem.thirdListElement}}</h5>
        <h5><i class="fas fa-chevron-right"></i>{{footerItem.fourthListElement}}</h5>
        <h5><i class="fas fa-chevron-right"></i>{{footerItem.fifthListElement}}</h5>
        <h5><i class="fas fa-chevron-right"></i>{{footerItem.sixthListElement}}</h5>
        
      </div>
      
    </div>
    
  </footer>
  <div class="bottom-footer">
      <h4>Enjoy the low price. we are tracking any intention of piracy</h4>
      <h4>marchio copyright 2020 NEXGEN is Proudly Powered by <span class="bottom-footer-decor">Codings</span></h4>
      

    </div>
    <div class="up-click">
      <i class="fas fa-arrow-up"></i>
    </div>
  </section>
        

</template>

<script>
export default {
  name: "Footer",
  data: function(){
      return {
          footerInfo:[
              {
                  title:"About",
                  firstListElement:"The Company",
                  secondListElement:"Institutional",
                  thirdListElement:"Social & Events",
                  fourthListElement:"Innovation",
                  fifthListElement:"Environment",
                  sixthListElement:"Technology"
              },
              {
                  title:"Services",
                  firstListElement:"Audit & Assurance",
                  secondListElement:"Financial Advisory",
                  thirdListElement:"Analytics M&A",
                  fourthListElement:"Middle Marketing",
                  fifthListElement:"Legal Consulting",
                  sixthListElement:"Regulatory Risk"
              },
              {
                  title:"Support",
                  firstListElement:"Responsibilty",
                  secondListElement:"Terms of Use",
                  thirdListElement:"About Cookies",
                  fourthListElement:"Privacy Policy",
                  fifthListElement:"Accessibility",
                  sixthListElement:"Information"
              },
              
              
              
          ]
      }
  }
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
        width: calc((100% / 4) - 20px);
        margin: 10px;
        padding: 7px;
        // height: 300px;
        
        .logo{
          margin: 10px 0;
          font-size: 21px;
        }
        .decor{
          padding: 5px 1px 5px 12px;
          border-top-left-radius: 20px;
          border-bottom-left-radius: 20px;
          background-color:#0e272d ;
          color:#00a4a0 ;
        }
        p{
          color: #b1bbbe;
          margin: 20px 0;
          font-size: 16px;
        }
        h4{
          margin: 10px 0;
          color: #b1bbbe;
          font-size: 14px;
          i{
            color:#bfc3d0 ;
          }
        }
        .btn{
          font-size: 18px;
          padding: 7px 14px;
          border: 1px solid #058283;
          margin: 18px 0 0;
          display: inline-block;
        }
      }
      .list{
        border-radius: 10px;
        background-color:#19191f ;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: left;
        padding-left:10px ;
        margin: 20px 0 0;
        max-height: 400px;
        h5{
          padding: 7px 0;
          font-size: 17px;
          color: #b1bbbe;
          i{
            margin-right: 6px;
          }
        }
        h3{
          font-size: 24px;
          margin-bottom: 10px;
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
    color: #b1bbbe;
    .bottom-footer-decor{
      color:#058283 ;
    }
  }
  .up-click{
    position: absolute;
    right: 16px;
    bottom: 10px;
    color: #0f1519;
    padding: 10px 12px;
    background-color:#1a1a1d ;
    border-radius: 50%;
  }
}
</style>