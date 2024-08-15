<template>
    <div v-on:click="counter">
        <h2>{{ name }}</h2>
        <p>{{ message }}</p>
        <p id="red">This item has been clicked {{ ctr }} times.</p>
    </div>
</template>

<script>
    export default{
        data(){
            return {
                name: 'Apples',
                message: 'I like apples',
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