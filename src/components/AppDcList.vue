<script>
    export default {
        data(){
             return{
                aboutDc :[
                    {
                        title:"DC COMICS",
                        list: ["Characters", "Comics", "Movies", "Tv", "Games", "Videos", "News"]
                    },
                    {
                        title:"SHOP",
                        list:["Shop DC", "Shop DC Collectibles"]
                    },
                    {
                        title:"DC",
                        list:["Terms of Use" , "Privacy  policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us" ]
                    },
                    {
                        title:"SITES",
                        list:["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
                    },
                ],
             }
        }

    }
</script>

<template>
    <section>
        <div class="container">
            <div class="list">
                <div v-for="(element, index) in aboutDc" key="element" class="row">          
                    <h3>{{ element.title }}</h3>
                    <ul v-for="(elements, index) in aboutDc[index].list" key="element" >
                        <li><a href="">{{elements }}</a></li>
                    </ul>          
                </div>
            </div>    
           <img src="../assets/img/dc-logo-bg.png" alt="">
   
        </div>    
    </section>
</template>

<style lang="scss" scoped>
section{
    height: 300px;
    background: url(../assets/img/footer-bg.jpg);
    color: white;
        .container{
            width: 80%;
            margin: auto;
            display: flex;
            justify-content: space-between;
            position: relative;
        
            .list{
            display: flex;

            
                .row:nth-child(2){
                    position: absolute;
                    bottom: 20px;
                    left:0;
                }
                .row{
                    margin:2rem ;
                   

                    ul{
                        list-style: none;
                        font-size: .8rem;

                        a{
                            text-decoration: none;
                            color: white;
                        }
                    }
                }

            }
            
            img{
                    object-fit: cover;
                    width: 30%;
                    height: 300px;
                }
        }   
}            
</style>