<template>
    <section>
        <div class="container">
            <div class="first-info">
                <div class="info">
                    <h4>OUR BUSINESS AREAS</h4>
                    <h2>Excellence in Services</h2>
                    <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowed professionals. These are some options that you can hire</p>
                </div>
                <div class="btn">
                    SEE ALL
                </div>
            </div>
            <div class="box-section">
                <!-- da popoplare con un array? -->
                <div class="single-box">

                </div>
                <div class="single-box">

                </div>
                <div class="single-box">

                </div>
                <div class="single-box">

                </div>
                <div class="single-box">

                </div>
                <div class="single-box">

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
    height: 800px;
    background-color: #eef4ed;
    padding:55px 0;
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
            }
        }
        .box-section{
            display: flex;
            flex-wrap: wrap;
            .single-box{
                width: calc((100% / 3) - 40px);
                // test
                height: 250px;
                background-color: pink;
                margin: 20px;
            }
        }       
    }
}
</style>