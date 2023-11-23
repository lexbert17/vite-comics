<script>
    export default {
        data(){
            return{
                content: "--> Content goes here <--"

            }
        }
    }
</script>

<template>
     <div class="biggest-container">
        <div class="container">
            <h2>{{ content }}</h2>
        </div>
     </div>    
</template>

<style lang="scss" scoped>
    .biggest-container{
    background-color: black;   
        .container{
            width: 80%;
            margin: auto;
            padding: 2rem 0;
            background-color: black;
            color: white;
        }
    }    
</style>