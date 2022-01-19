<template>
  <section>
    <div class="col sinistra">
      <div class="top-info">
        <h4>ABOUT THE NETWORK</h4>
        <h2><span class="decor">The</span> Company</h2>
        <p>for 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients</p>
      </div>
      <div class="info-container">
       
        <div class="info-card">
          <h2><i class="fas fa-ribbon"></i>Tradition </h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <div class="info-card">
          <h2><i class="fas fa-lock"></i>Security </h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <div class="info-card">
          <h2><i class="far fa-edit"></i>Certificate </h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        <div class="info-card">
          <h2><i class="fas fa-graduation-cap"></i>Expertise</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
        
        
      </div>
      <div >
        <span class="btn">GET IN TOUCH</span><span class="btn">READ MORE</span>
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
  // height:700px ;
  position: relative;
  
  // test
  color: white;
  background-color: black;
  .col{
    width: 50%;
    .btn{
        margin: 20px 10px;
        padding: 7px 17px;
        border: 1px solid #058283 ;
        display: inline-block;
        cursor: pointer;
        &:hover{
          background-color: #058283 ;
          transition: 0.3s;
        }
      }
    .top-info{
      h4{
        font-size: 10px;
        color:#039293 ;
      }
      h2{
        font-size: 40px;
        margin: 17px 0;
        .decor{
          background-color:#0e272d ;
          padding: 4px 9px;
        }
      }
      p{
        color: #888a94;
        font-size: 14px;
        margin: 17px 0;
      }
    }
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
        display: flex;
        flex-direction: column;
        justify-content: center;
        
        // test
       
        height: 65%;
        h2{
          font-size: 19px;
          padding: 10px 0;
          i{
            color:#039293  ;
          }
        }
        p{
          color: #888a94;
        }
      }
    }
  }
  .sinistra{
    width: 30%;
    margin:10% 5% 4% 20% ;
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
  .bottom{
    transform: translate(-50% , 0);
    bottom: -35px;
    left: 50%;
  }
}
</style>