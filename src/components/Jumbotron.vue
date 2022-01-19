<template>
    <section>
        <div class="background-image">
            <div class="container">
                <div class="sinistra">
                    <img src="../assets/img/logo.png" alt="">
                </div>
                <div class="destra">
                    <ul>
                        <li>HOME</li>
                        <li>SERVICES</li>
                        <li>ABOUT</li>
                        <li>PROJECTS</li>
                        <li>RESULTS</li>
                        <li>GET IN TOUCH</li>
                    </ul>
                </div>
            </div>
            <div class="central-text">
                <h2>Ready <span class="decor">Team</span></h2>
                <p>no matter what your company needs, we will be ready to assist you in the best possible way.</p>
                <div>
                    <span class="btn">
                    GET IN TOUCH
                </span>
                <span class="btn">
                    READ MORE
                </span>
                </div>

            </div>
        </div>
        <div class="decor-elements">
            <div class="empty">

            </div>
            <div class="full">

            </div>
            <div class="empty">

            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: "Jumbotron",
  
};
</script>


<style scoped lang="scss">
section{
    height: 600px;
    position: relative;
    .background-image{
        background-image: url("../assets/img/bg-parallax.png");
        background-position: center ;
        background-size: 170%;
        background-repeat: no-repeat;
        height: 100%;
        overflow: hidden;
        .container{
        width: 70%;
        height: 40px;
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        line-height: 40px;
        font-size: 15px;
        padding:30px 0;
        min-width: 700px;
        .sinistra{
            padding-top:10px ;
            img{
                width: 100px;
            }
            
        }
        .destra{
            ul{
            list-style-type: none;
            display: flex;
            flex-direction: row;
            li{
                cursor: pointer;
                padding: 3px 10px;
                &:hover{
                    color: white;
                    background-color:#058283 ;
                    border-radius: 4px;
                    transition: 0.7s;
                }
            }
        }
        }
    }
        .central-text{
            width: 25%;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            margin: auto;
            text-align: center;
            padding: 10px;
            h2{
                font-size: 60px;
                margin: 20px 0;
                font-weight: bold;
                color:#21333e ;
                .decor{
                    color:#058283 ;
                    background-color: #d5e7e8;
                    padding: 5px 9px;
                }
            }
            p{
                font-size: 16px;
                color:#8c969b ;
                margin-bottom:30px ;
            }
            .btn{
                padding: 7px 17px;
                border: 1px solid #058283;
                color: #058283;
                cursor: pointer;
                margin: 0 11px;
                font-size: 15px;
                font-weight: bold;
                display: inline-block;
                &:hover{
                    background-color: #058283;
                    color: white;
                    transition: 0.5s;
                }
            }
        }
    }
    .decor-elements{
        display: flex;
        flex-direction: column;
        position: absolute;
        top: 50%;
        left: 95%;
        transform: translate(-50% , -5%);
        
        .empty{
            border: 2px solid #a0d5d8;
            padding: 17px 4px;
            border-radius: 20px;
            margin: 5px 0;
        }
        .full{
            border: 1px solid #058283;
            padding: 20px 3px;
            border-radius: 20px;  
            background-color:#058283 ;
        }
    }
}
</style>