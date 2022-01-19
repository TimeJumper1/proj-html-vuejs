<template>
    <section>
        <div class="container">
            <div class="first-info">
                <div class="info">
                    <h4>OUR BUSINESS AREAS</h4>
                    <h2>Excellence in <span class="decor">Services</span></h2>
                    <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowed professionals. These are some options that you can hire</p>
                </div>
                <div class="btn">
                    SEE ALL
                </div>
            </div>
            <div class="box-section">
                <!-- da popoplare con un array -->
                <div v-for="(servicesItem, index) in servicesInfo" :key="index" class="single-box">
                    <div class="top-part">
                        <div>
                            <i :class="servicesItem.icon"></i>
                        </div>
                        <div class="arrow">
                            <i :class="servicesItem.arrowIcon"></i>
                        </div>
                    </div>
                    <h3>{{servicesItem.title}}</h3>
                    <p>{{servicesItem.content}}</p>
                </div>
                
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: "ServiceSection",
  data: function(){
      return {
          servicesInfo:[
              {
                  icon:"fas fa-network-wired",
                  arrowIcon: "fas fa-arrow-right",
                  title:"Audit & Insurance",
                  content:"Lorem ipsum dolor, sit amet consectetur adipisicing elit."
              },
              {
                  icon:"fas fa-briefcase",
                  arrowIcon: "fas fa-arrow-right",
                  title:"Financial Advisory",
                  content:"Lorem ipsum dolor, sit amet consectetur adipisicing elit."
              },
              {
                  icon:"far fa-chart-bar",
                  arrowIcon: "fas fa-arrow-right",
                  title:"Analytics and M&A",
                  content:"Lorem ipsum dolor, sit amet consectetur adipisicing elit."
              },
              {
                  icon:"fas fa-rocket",
                  arrowIcon: "fas fa-arrow-right",
                  title:"MIddle Marketing",
                  content:"Lorem ipsum dolor, sit amet consectetur adipisicing elit."
              },
              {
                  icon:"fas fa-globe",
                  arrowIcon: "fas fa-arrow-right",
                  title:"Legal Consulting",
                  content:"Lorem ipsum dolor, sit amet consectetur adipisicing elit."
              },
              {
                  icon:"fas fa-inbox",
                  arrowIcon: "fas fa-arrow-right",
                  title:"Regulatory Risk",
                  content:"Lorem ipsum dolor, sit amet consectetur adipisicing elit."
              },
          ]
      }
  }
};
</script>


<style scoped lang="scss">
section{
    // height: 800px;
    background-color: #eef4ed;
    padding: 40px 0;
    .container{
        width: 70%;
        margin: auto;
        .first-info{
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: flex-end;
            .info{
                width: 70%;
                padding: 6px;
                h4{
                    color:#058283  ;
                    font-size: 10px;
                }
                h2{
                    font-size: 37px;
                    color:#21333e ;
                    .decor{
                        color: #058283 ;
                        background-color:#cce3de ;
                        padding: 4px 9px;
                    }
                }
                p{
                    font-size: 14px;
                    color:#8c969b  ;
                    padding:18px 0  ;
                }
            }
            .btn{
                padding: 7px 17px;
                cursor: pointer;
                color: white;
                background-color:#058283 ;
                border-radius: 3px;
                margin-bottom: 20px;
            }
        }
        .box-section{
            display: flex;
            flex-wrap: wrap;
            .single-box{
                width: calc((100% / 3) - 40px);
                display: flex;
                flex-direction: column;
                justify-content: center;
                height: 200px;
                background-color: white;
                margin: 20px;
                text-align: center;
                border-radius: 7px;
                .top-part{
                    display: flex;
                    justify-content: space-between;
                    padding: 20px;
                    color:#058283 ;
                    font-size: 28px;
                    .arrow{
                        color:#83c1c1 ;
                        padding: 7px 12px;
                        border-radius: 30px;
                        &:hover{
                            color: #0c8788;
                            background-color: #7bd1d1;
                            transition: 0.3s;
                        }
                    }
                }
                h3{
                    font-size: 22px;
                    padding: 7px;
                }
                p{
                    font-size: 17px;
                    color:#8c969b  ;
                }
            }
        }       
    }
}
</style>