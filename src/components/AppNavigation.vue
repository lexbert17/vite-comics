<script>
    export default {
        data(){
            return{
                imgAndElement :[
                    {
                        image:"buy-comics-digital-comics.png",
                        element:"DIGITAL COMICS"
                    },
                    {
                        image:"buy-comics-merchandise.png",
                        element:"DC MERCHANDISE"
                    },
                    {
                        image:"buy-comics-subscriptions.png",
                        element:"SUBSCRIPTION"
                    },
                    {
                        image:"buy-comics-shop-locator.png",
                        element:"COMIC SHOP LOCATOR"
                    },
                    {
                        image:"buy-dc-power-visa.svg",
                        element:"DC POWER VISA"
                    },
                ],
            };
        },
        methods: {
            getImagePath: function(img) {
                return new URL(`../assets/img/$(img)`, import.meta.url).href;
            }
        }
    };
</script>

<template>
<div class="biggest-container">   
    <div  class="container">
        <ul v-for="part in imgAndElement">
            <li>
                
                   <a  href="">
                    <img  :src="getImagePath(imgAndElement.image)" alt="img"><span>{{ part.element }}</span>
                   </a>   
            </li>
        </ul>
       
  
    </div> 
</div>       
</template>

<style lang="scss" scoped>
.biggest-container{
    background-color:  hsl(208.67deg 100% 48.82%);
    .container{
    background-color: hsl(208.67deg 100% 48.82%);
    color: white;
    width: 80%;
    margin: auto;
    padding: 2.5rem 1rem;
    justify-content: center;

        ul{
        list-style: none;
        display: flex;
        gap: 3rem;
        justify-content: center; 
        
        }   
            a{
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;

                    img{
                    width: 2rem;
                    margin-right: 1rem;
                    }

            }   
    }

}
</style> 