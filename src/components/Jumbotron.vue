<template>
    <section>
        <div class="background-image">
            <div class="container">
                <div class="sinistra">
                    testo
                </div>
                <div class="destra">
                    <ul>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                        <li>test</li>
                    </ul>
                </div>
            </div>
            <div class="central-text">
                <h2>Ready Team</h2>
                <p>no matter what your company needs, we will be ready to assist you in the best possible way.</p>
                <span class="btn">
                    get in touch
                </span>
                <span class="btn">
                    get in touch
                </span>

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
    position: relative;
    height: 500px;
    .background-image{
        background-image: url("../assets/img/bg-parallax.png");
        background-position: center ;
        background-size: 150%;
        background-repeat: no-repeat;
        height: 100%;
        overflow: hidden;
        .container{
        width: 70%;
        margin: auto;
        display: flex;
        justify-content: space-between;
        line-height: 40px;
        ul{
            list-style-type: none;
            display: flex;
            flex-direction: row;
            li{
                margin:0 10px;
            }
        }
    }
        .central-text{
            width:20% ;
            position: absolute;
            top: 50%;
            left: 40%;
            text-align: center;
            padding: 10px;
            font-size: 20px;
        }
    }
    
}
</style>