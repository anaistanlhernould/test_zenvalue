<template>
    <div class="modele_div">
        <input type="text" v-model="message"> 
        <p> {{message}} </p> 
    </div>
</template>

<script>
    export default {
        data () {
            return{
                message: " Contenu de ma div ",
            }
        },
        
        
    }
</script>

<style>
    .modele_div{
        background: rgb(241, 240, 240); 
        width : 20%; 
        height : auto; 
        border : 0.5px solid #000; 
        margin: 20px; 
        padding: 20px; 
    }
</style>