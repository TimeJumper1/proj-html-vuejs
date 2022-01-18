<template>
    <section>
        <div class="top-info">
            <h5>WE DO MORE FOR EVERYONE</h5>
            <h2>Action & projects</h2>
            <ul>
                <li>all</li>
                <li>all</li>
                <li>all</li>
                <li>all</li>
                <li>all</li>
                <li>all</li>
                <li>all</li>
            </ul>
        </div>
        <div class="foto-section">
            <!-- da popolarecon un v-for -->
            <div class="foto-card">
                <img src="../assets/img/project-1.jpg" alt="mani sul computer">
                <h3>testo per vedere se tutto va</h3>
            </div>
            <div class="foto-card">
                <img src="../assets/img/project-2.jpg" alt="mani sul computer">
                <h3>testo per vedere se tutto va</h3>
            </div>
            <div class="foto-card">
                <img src="../assets/img/project-3.jpg" alt="mani sul computer">
                <h3>testo per vedere se tutto va</h3>
            </div>
            <div class="foto-card">
                <img src="../assets/img/project-4.jpg" alt="mani sul computer">
                <h3>testo per vedere se tutto va</h3>
            </div>
            <div class="foto-card">
                <img src="../assets/img/project-5.jpg" alt="mani sul computer">
                <h3>testo per vedere se tutto va</h3>
            </div>
            <div class="foto-card">
                <img src="../assets/img/project-6.jpg" alt="mani sul computer">
                <h3>testo per vedere se tutto va</h3>
            </div>

        </div>
    </section>
</template>

<script>
export default {
  name: "ActionSection",
  
};
</script>


<style scoped lang="scss">
section{
    margin: 100px 0;
    .top-info{
        text-align: center;
        ul{
            list-style-type: none;
            display: flex;
            justify-content: center;
            li{
                margin: 3px 10px;
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
            }
        }

    }
}
</style>