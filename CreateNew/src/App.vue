<script>
export default{
  data(){
    return{
      message: 'This is some Text'
    };
  }
}

</script>

<template>
  <h1>Food</h1>
  <food-item food-name="Apples" food-desc="An apple a day keeps the doctor away" v-bind:is-favourite="true"/>
  <food-item food-name="Pizza" food-desc="Pizza is a fast-food"v-bind:is-favourite="true"/>
  <food-item food-name="Rice" food-desc="Rice is a grain"v-bind:is-favourite="true"/>
  
</template>

<style>
#app>div{
  border: dashed black 1px;
  display: inline-block;
  margin: 10px;
  padding: 10px;
  background-color: lightgreen;
  cursor: pointer;
}

</style>
