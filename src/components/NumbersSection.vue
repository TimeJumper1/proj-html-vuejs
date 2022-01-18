<template>
    <section>
        <div class="top-part">
            <div class="container">
                <h4>WHAT ARE WE DOING</h4>
                <h2>Results in Numbers</h2>
                <div class="numbers">
                    <!-- da fare un con un v-for -->
                    <div class="single-number">
                        <h2>128</h2>
                        <h3>certifications</h3>
                    </div>
                    <div class="single-number">
                        <h2>128</h2>
                        <h3>certifications</h3>
                    </div>
                    <div class="single-number">
                        <h2>128</h2>
                        <h3>certifications</h3>
                    </div>
                    <div class="single-number">
                        <h2>128</h2>
                        <h3>certifications</h3>
                    </div>
                </div>
    
            </div>
        </div>
        <div class="bottom-part">
            <div class="partners">
                <!-- andranno resizati tutti -->
                <img src="../assets/img/logo-4.png" alt="logo jQuery">
                <img src="../assets/img/logo-5.png" alt="logo jQuery">
                <img src="../assets/img/logo-1.png" alt="logo jQuery">
                <img src="../assets/img/logo-2.png" alt="logo jQuery">
                <img src="../assets/img/logo-3.png" alt="logo jQuery">
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: "NumbersSection",
  
};
</script>


<style scoped lang="scss">
section{
    height: 700px;
    background-color: pink;
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
            
            .numbers{
                display: flex;
                flex-direction: row;
                justify-content: space-evenly;
                margin: 60px 0;
            }
        }
        
    }
    .bottom-part{
        height: 250px;
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
                filter: invert(100%);
            }
        }
    }

}
</style>