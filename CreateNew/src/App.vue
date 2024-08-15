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
  <food-item/>
  <food-item/>
  <food-item/>
  
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
