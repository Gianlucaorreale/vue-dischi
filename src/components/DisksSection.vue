<template>
  <section id="disks"></section>
</template>

<script>
import axios from 'axios';
export default{
    name: 'DisksSection',
    mounted(){
        axios.get('https://flynn.boolean.careers/exercises/api/array/music').then(()=>{})
    }
}
</script>

<style>

</style>