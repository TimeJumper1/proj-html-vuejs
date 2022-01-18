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
                <div class="single-box">
                    <div class="top-part">
                        <div>
                            <i class="fas fa-network-wired"></i>
                        </div>
                        <div class="arrow">
                            <i class="fas fa-arrow-right"></i>
                        </div>
                    </div>
                    <h3>Audit & assurance</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. </p>
                </div>
                <div class="single-box">
                    <div class="top-part">
                        <div>
                            <i class="fas fa-briefcase"></i>
                        </div>
                        <div class="arrow">
                            <i class="fas fa-arrow-right"></i>
                        </div>
                    </div>
                    <h3>Financial Advisory</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. </p>
                </div>
                <div class="single-box">
                    <div class="top-part">
                        <div>
                            <i class="far fa-chart-bar"></i>
                        </div>
                        <div class="arrow">
                            <i class="fas fa-arrow-right"></i>
                        </div>
                    </div>
                    <h3>Analytics and M&A</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. </p>
                </div>
                <div class="single-box">
                    <div class="top-part">
                        <div>
                            <i class="fas fa-rocket"></i>
                        </div>
                        <div class="arrow">
                            <i class="fas fa-arrow-right"></i>
                        </div>
                    </div>
                    <h3>Middle Marketing</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. </p>
                </div>
                <div class="single-box">
                    <div class="top-part">
                        <div>
                            <i class="fas fa-globe"></i>
                        </div>
                        <div class="arrow">
                            <i class="fas fa-arrow-right"></i>
                        </div>
                    </div>
                    <h3>Legal Consulting</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. </p>
                </div>
                <div class="single-box">
                    <div class="top-part">
                        <div>
                            <i class="fas fa-inbox"></i>
                        </div>
                        <div class="arrow">
                            <i class="fas fa-arrow-right"></i>
                        </div>
                    </div>
                    <h3>Regulatory Risk</h3>
                    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: "ServiceSection",
  
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