<template>
    <div v-on:click="counter" >
        <h2>{{ foodName }}</h2>
        <img src="" v-show="isFavourite">
        <p>{{ foodDesc }}</p>
        <p id="red">This item has been clicked {{ ctr }} times.</p>
    </div>
</template>

<script>
    export default{
        // props:[
        //     'foodName',
        //     'foodDesc',
        //     'isFavourite'
        // ],

        props:{
            foodName: String,
            foodDesc: String,
            isFavourite: Boolean
        },
        data(){
            return{
                ctr:0
            }            
        },
        methods:{
            counter(){
                this.ctr++;
            }
        }
    }
</script>

<style>
    #red{
        font-weight:bold;
        color: red;
    }
</style>