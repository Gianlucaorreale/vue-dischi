<template>
   <div class="disk-card text-center p-2">
      <img :src="image" :alt="name" class="image-fluid mb-3">
      <h2>{{name}}</h2>
      <div class="group">{{group}}</div>
      <div class="year">{{year}}</div>
   </div>
</template>

<script>
  export default {
    name:'DiskCard',
    props: {
      name: String,
      image: String,
      group: String,
      year: String
    }
  }
</script>

<style lang="scss" scoped>
.disk-card{
    width: 20%;
}

img{
    height: 200px;
}
</style>