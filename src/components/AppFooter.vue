<script>
    export default {
        data() {
            return{

            }
        }
    }
</script>

<template>
    <section>
        <div class="container">
            <button><h4>SIGN-UP NOW!</h4></button>
            <div class="icons">
                <h4>FOLLOW US</h4>
                <a href="">
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </a>    
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    section{
        background-color: hsl(0deg 0% 18.82%);

        .container{
            width: 80%;
            margin: auto;
            display: flex;
            justify-content: space-between;
        }

            button{
                height: 30px;
                display: block;
                align-self: center;
                border: 2px solid hsl(210.41deg 74.75% 61.18%)  ;
                background-color: hsl(0deg 0% 18.82%) ;
                color: white;
                padding: 0px 10px ;

                &:hover{
                    filter: brightness(1.75);
                }
            }

            .icons{
                display: flex;
                justify-content: space-between;
                align-items: center;

                h4{
                    color: hsl(210.41deg 74.75% 61.18%);
                    margin-right: 0.5rem;
                }

                img{
                    width: 30px;
                    margin: 1rem .5rem;
                }
            }
    }
</style>