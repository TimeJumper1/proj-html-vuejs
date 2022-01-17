<template>
    <header>
        <div class="container">
            <div class="destra">
                orario
            </div>
            <div class="sinistra">
                <ul>
                    <li>info</li>
                    <li>info</li>
                    <li>info</li>
                    <li>info</li>
                    <li>info</li>
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
</style>