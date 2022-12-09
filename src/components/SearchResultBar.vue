<template>
    <div id="result_bar">
        <div class="info">
            <p>國立臺灣博物館_鐵道部園區</p>
            <p>地址: 103 臺北市大同區延平北路一段2號</p>
        </div>
        
        <div class="fav_icon">
            <img v-if="faved == false" src="favicon_url" alt="fav" width="60" v-on:click="change_favicon">
            <img v-if="faved == false" src="favicon_url" alt="fav" width="60" v-on:click="change_favicon">
        </div>
    </div>
</template>

<script>
const vm = Vue.createApp({
    data(){
        return{
            avicon_url: '..\assets\favourite.png',
            faved:false
        }
    },
    methods:{
        change_favicon: function() {
            this.faved = true

        }
    }
}).mount('#result_bar')


</script>

<style scoped>
/* body{
    margin: 0;
    padding: 0;
} */
#result_bar{
    border: solid 2px #93827F;
    padding: 2px;
    height: 80px;
    display: flex;
    
}

.fav_icon{
    width: 60px;
    height: 60px;
    /* border: solid 1px black; */
    /* border-radius: 99em;  */
    display: inline-flex;
    justify-content: center; 
    align-items: center; 
    margin-left: 60%;
    margin-top: 5px;
}
</style>