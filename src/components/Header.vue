<template>
    <header>
        <div class="container">
            <div class="sinistra">
                <i class="fas fa-clock"></i>
                Open Hours: Mon - Sat - 9:00 - 18:00
            </div>
            <div class="destra">
                <ul>
                    <li><i class="fas fa-phone-alt"></i>+1 (305) 1234-5678</li>
                    <li><i class="fas fa-envelope"></i>Hello@example.com</li>
                    <li><i class="fab fa-facebook-f"></i></li>
                    <li><i class="fab fa-twitter"></i></li>
                    <li><i class="fab fa-linkedin-in"></i></li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String,
  },
};
</script>


<style scoped lang="scss">
header{
    background-color: #21333e;
    height: 40px;
    color: white;
    .container{
        width: 70%;
        margin: auto;
        display: flex;
        justify-content: space-between;
        line-height: 40px;
        min-width: 700px;
        .sinistra{
            font-size: 13px;
            color:#c0c3d0 ;
        }
        .destra{
            font-size: 13px;
            color:#c0c3d0 ;
            ul{
            list-style-type: none;
            display: flex;
            flex-direction: row;
            li{
                margin:0 10px;
            }
        }
        }
    }
}
</style>