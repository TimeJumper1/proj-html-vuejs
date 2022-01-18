<template>
    <section>
        <div class="container">
            <div class="form">
                <div>
                    <h4>SEND A MESSAGE</h4>
                    <h2>Get in Touch</h2>
                    <p>we will respond ti your message as soon as possible</p>
                </div>
                <div class="inputs">
                    <input type="text" placeholder="name">
                    <input type="text" placeholder="name">
                    <br>
                    <input type="text" placeholder="name">
                    <select name="" id="" placeholder="name">
                        <option value="">a</option>
                        <option value="">a</option>
                        <option value="">a</option>
                        <option value="">a</option>
                    </select>
                    <br>
                    <textarea name="" id="" cols="30" rows="10" placeholder="message"></textarea>
                </div>
            </div>
            <div class="examples">
                <h3>examples</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil distinctio enim, ipsam quibusdam odio cumque eos culpa illum beatae porro ducimus accusamus fuga ha</p>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rerum, maxime! Architecto numquam reiciendis quia natus reprehenderit blanditiis incidunt sed rem dicta, sint aut voluptatibus quos minus obcaecati doloribus </p>
                <h2>immagine + numero di telefono</h2>
                <h2>immagine + numero di telefono</h2>
                <h2>immagine + numero di telefono</h2>
                <span>
                    bottone
                </span>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: "FormSection",
  
};
</script>


<style scoped lang="scss">
section{
    height: 700px;
    .container{
        width: 70%;
        height: 100%;
        margin: auto;
        display: flex;
        flex-direction: row;
        align-items: center;
        .form{
            width: 60%;
            
            
        }
        .examples{
            width: 40%;
            
            
            
        }
    }

}
</style>