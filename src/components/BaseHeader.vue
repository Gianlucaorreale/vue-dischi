<template>
  <header>
    <h1>{{heading}}</h1>
  </header>
</template>

<script>
 export default{
  name: 'BaseHeader',
  props:{
    heading: {
        type: String,
        required: true
    }
  }
 } 
</script>

<style>
header{
    background-color: #2E3A46;
}

 h1{
    color: #1ED760;
}
</style>