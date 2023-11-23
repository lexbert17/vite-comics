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
    <div class="container">
        <h2>{{ content }}</h2>
    </div>
</template>

<style lang="scss" scoped>
    .container{
        width: 80%;
        margin: auto;
        padding: 1.5rem 0;
        background-color: yellow;
    }
</style>