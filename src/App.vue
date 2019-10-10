<template>
    <div id="app">
        <button @click="addDiv()" class="style_button">
            Cliquez ici pour ajouter une DIV
        </button>
        <mydiv v-drag v-for="n in range" :key="n">
        </mydiv>
    </div>
</template>

<script>

/* importation de la div */
import mydiv from './mydiv.vue'
    export default {
        name: 'app', 
        components: {
            mydiv, 
        },
        data() {
            return{
                range:0,
            }
        }, 
        methods: {
        addDiv: function(){
            this.range += 1; 
        }
    },
    }

/* DRAG AND DROP */
Vue.use(vdrag);
import Vue from 'vue';
import vdrag from 'v-drag';

</script>

<style>
.center{
    margin : 0 auto; 
    text-align: center; 
}

.style_button{
    background: rgb(1, 12, 36); 
    color : #fff; 
    font-size: 0.8em; 
    padding : 10px; 
    border : none; 
}
</style>

