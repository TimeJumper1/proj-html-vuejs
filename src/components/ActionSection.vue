<template>
    <section>
        <div class="top-info">
            <h5>WE DO MORE FOR EVERYONE</h5>
            <h2>Action & <span class="decor">Projects</span></h2>
            <ul>
                <li>ALL</li>
                <li>INSTITUTIONAL</li>
                <li>SOCIAL</li>
                <li>EVENTS</li>
                <li>INNOVATION</li>
                <li>ENVIRONMENT</li>
                <li>TECHNOLOGY</li>
            </ul>
        </div>
        <div class="foto-section">
            <!-- da popolarecon un v-for -->
            <div v-for="(actionItem, index) in actionInfo" :key="index" class="foto-card">
                <img :src="require(`../assets/img/project${actionItem.image}.jpg`)" alt="foto 1">
                <h3>{{actionItem.content}}</h3>
            </div>
            

        </div>
    </section>
</template>

<script>
export default {
  name: "ActionSection",
  data: function(){
      return {
          actionInfo:[
              {
                  image:"-1",
                  content:"Academic professional program in social media"
              },
              {
                  image:"-2",
                  content:"President's speech at the annual meeting"
              },
              {
                  image:"-3",
                  content:"International business trip in Shanghai"
              },
              {
                  image:"-4",
                  content:"Technology workshop with education theme"
              },
              {
                  image:"-5",
                  content:"Donation of clothes and food to the partner NGO"
              },
              {
                  image:"-6",
                  content:"Confraternization of the procurement team"
              },
              
          ]
      }
  }
};
</script>


<style scoped lang="scss">
section{
    margin: 100px 0;
    .top-info{
        text-align: center;
        h5{
            font-size: 10px;
            color:#1ba8a7 ;
        }
        h2{
            font-size: 33px;
            margin: 30px;
            .decor{
                color: #058283;
                background-color: #daeced;
                padding: 7px 17px;
                border-radius: 4px;
            }
        }
        ul{
            list-style-type: none;
            display: flex;
            justify-content: center;
            margin: 8px 20px;
            li{
                
                padding: 6px 14px;
                color: #66727a;
                border-radius: 3px;
                &:hover{
                    background-color: #daeced;
                    transition: 0.3s;
                }
            }
        }
    }
    .foto-section{
        display: flex;
        flex-wrap: wrap;
        flex-direction: row;
        width: 70%;
        margin: auto;
        .foto-card{
            width: calc((100% / 3) - 10px);
            height: auto;
            border-radius: 20px;
            
            overflow: hidden;
            margin: 5px;
            position: relative;
            img{
                max-width: 100%;
                max-height:100% ;
                filter: brightness(50%);
            }
            h3{
                position: absolute;
                text-align: center;
                color: white;
                left: 50%;
                top: 70%;
                transform: translate(-50% , -30%);
                width: 80%;
                min-width: 200px;
                font-size: 22px;
            }
        }

    }
}
</style>