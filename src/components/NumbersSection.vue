<template>
    <section>
        <div class="top-part">
            <div class="container">
                <h4>WHAT ARE WE DOING</h4>
                <h2 class="title"><span class="decor"> Results</span> in Numbers</h2>
                <div class="numbers">
                    <!-- da fare un con un v-for -->
                    <div v-for="(numberItem, index) in numberInfo" :key="index" class="single-number">
                        <h2>{{numberItem.number}}</h2>
                        <h3>{{numberItem.content}}</h3>
                    </div>
                    <!-- <div class="single-number">
                        <h2>280</h2>
                        <h3>Employees</h3>
                    </div>
                    <div class="single-number">
                        <h2>517</h2>
                        <h3>Customers</h3>
                    </div>
                    <div class="single-number">
                        <h2>94</h2>
                        <h3>Country Served</h3>
                    </div> -->
                </div>
    
            </div>
        </div>
        <div class="bottom-part">
            <div class="partners">
                <!-- andranno resizati tutti -->
                <img class="outlier" src="../assets/img/logo-4.png" alt="logo jQuery">
                <img class="outlier" src="../assets/img/logo-5.png" alt="logo jQuery">
                <img src="../assets/img/logo-1.png" alt="logo jQuery">
                <img src="../assets/img/logo-2.png" alt="logo jQuery">
                <img src="../assets/img/logo-3.png" alt="logo jQuery">
                <img class="outlier" src="../assets/img/logo-4.png" alt="logo jQuery">
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: "NumbersSection",
  data: function(){
      return {
          numberInfo:[
              {
                  number:"128",
                  content:"certifications"
              },
              {
                  number:"230",
                  content:"Employees"
              },
              {
                  number:"517",
                  content:"Customers"
              },
              {
                  number:"94",
                  content:"Countries Served"
              },
              
              
          ]
      }
  }
};
</script>


<style scoped lang="scss">
section{
    height: 700px;
    
    .top-part{
        background-image: url("../assets/img/bg-7.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        height:450px;
        color: white;
        display: flex;
        flex-direction: column;
        justify-content:center ;
        .container{
            width: 70%;
            margin: auto;
            text-align: center;
            h4{
                color:#038f7f ;
                font-size: 12px;
            }
            .title{
                font-size: 44px;
                margin: 24px 0;
                .decor{
                    background-color: #0c2c2e;
                    padding: 4px 9px;
                }
            }
            .numbers{
                display: flex;
                flex-direction: row;
                justify-content: space-evenly;
                margin: 60px 0;
                h2{
                    font-size: 33px;
                    color: #01a5a6;
                    margin: 10px;
                }
                h3{
                    font-size: 20px;
                }
            }
        }
        
    }
    .bottom-part{
        height: 200px;
        background-color: #111117;
        .partners{
            width: 70%;
            height: 100%;
            margin: auto;
            display: flex;
            flex-direction: row;
            justify-content: space-evenly;
            align-items: center;
            img{
                width: 9%;
                filter: invert(50%);
                
            }
            .outlier{
                width: 5%;
            }
        }
    }

}
</style>