<script>
    export default {
        data() {
            return {
                navHeader: [ "CHARACTERS", "COMICS", "MOVIES", "TV", "GAMES", "COLLECTIBLES", "VIDEOS", "FANS", "NEWS", "SHOP"]
            }
        }
    }
</script>

<template>
    <header>
        <div class="container">
            <div>
                <img src="../assets/img/dc-logo.png" alt="img">
            </div>
            <ul>
                <li v-for="item in navHeader"><a href="">{{ item }}</a></li>
            </ul>
        </div>    
    </header>
</template>

<style lang="scss" scoped>
.container{
    display: flex;
    width: 80%;
    margin: auto;
    justify-content: space-between;
    margin: auto;
    background-color: green;
    height: 120px;
    align-items: center;
    
  
    img {
        width: 80px;
    }

    ul {
        display: flex;
        gap: 1rem;
        list-style: none;
        background-color: orange;
        height: 100%;
        

        a {
        color: black;
        text-decoration: none;
        display: block;
        line-height: 120px;
        height: 120px;
       
        

            &:hover {
                color: hsl(208.67deg 100% 48.82%);
                border-bottom: 5px solid hsl(208.67deg 100% 48.82%);
         
            }
          
        }
    }
};   
</style> 