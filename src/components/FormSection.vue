<template>
    <section>
        <div class="container">
            <div class="form">
                <div>
                    <h4>SEND A MESSAGE</h4>
                    <h2>Get in <span class="decor">Touch</span></h2>
                    <p>we will respond ti your message as soon as possible</p>
                </div>
                <div class="inputs">
                    <input type="text" placeholder="name">
                    <input type="text" placeholder="name">
                    <br>
                    <input type="text" placeholder="name">
                    <select name="more info" id="" >
                        <option value="">more info</option>
                        <option value="">a</option>
                        <option value="">a</option>
                        <option value="">a</option>
                    </select>
                    <br>
                    <textarea name="" id="" cols="150" rows="10" placeholder="message"></textarea>
                    <br>
                    <span class="btn">SEND</span>
                </div>
            </div>
            <div class="examples">
                <h3>examples Inc.</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.  </p>
                <h2><span class="circle"><i class="fas fa-phone-alt"></i></span> +1 (305) 1234-5678</h2>
                <h2><span class="circle"><i class="fas fa-envelope"></i></span>hello@example.com</h2>
                <h2><span class="circle"><i class="fas fa-map-marker-alt"></i></span>Main Avenue, 987</h2>
                <span class="btn">
                    VIEW MAP
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
            h4{
                color:#10aaae ;
                font-size: 10px;
            }
            h2{
                font-size: 38px;
                color: #21333e;
                margin: 20px 0;
                .decor{
                    color:#058283 ;
                    background-color:#daeced ;
                    padding: 5px 8px;
                }
            }
            p{
                color: #a6abb0;
                font-size: 13px;  
                margin: 20px 0; 
            }
            .inputs{
                input{
                    padding: 8px 11px;
                    background-color:#ececec ;
                    border-radius: 4px;
                    outline: none;
                    border: none;
                    margin: 7px 7px 7px 0 ;
                    width: calc((100% / 2) - 20px);
                }
                select{
                    padding: 8px 11px;
                    background-color:#ececec ;
                    border-radius: 4px;
                    outline: none;
                    border: none;
                    margin: 7px 7px 7px 0 ;
                    width: calc((100% / 2) - 20px);
                    color: #817d80;
                    option{
                        color:#ececec ;
                    }
                }
                textarea{
                    max-width: 95%;
                    padding: 8px 11px;
                    margin: 7px 7px 27px 0 ;
                    background-color:#ececec ;
                    border-radius: 4px;
                    outline: none;
                    border: none;
                }
                .btn{
                    padding: 7px 18px;
                    border: 1px solid #058283;
                    color: #058283;
                    cursor: pointer;
                    border-radius:4px ;
                    &:hover{
                        background-color:#058283 ;
                        color: white;
                        transition: 0.3s;
                    }
                }
            }
        }
        .examples{
            width: 40%;
            padding-bottom: 170px;
            h3{
                font-size: 23px;
                margin: 26px 0;
                color: #213340;
            }  
            p{
               color: #a6abb0; 
               font-size: 15px;
               margin: 26px 0;
            }  
            h2{
                color:#058283 ;
                margin: 30px 0;
                font-size: 16px;
                .circle{
                    padding: 5px;
                    border-radius: 50%;
                    background-color:#daeced ;
                }
            }
            .btn{
                padding: 7px 18px;
                border: 1px solid #058283;
                color: #058283;
                cursor: pointer;
                border-radius:4px ;
                &:hover{
                    background-color:#058283 ;
                    color: white;
                    transition: 0.3s;
                }
            }
        }
    }

}
</style>