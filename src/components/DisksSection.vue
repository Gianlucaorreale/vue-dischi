<template>
  <section id="disks">
    <div class="disks-list gy-4 d-flex flex-wrap">
        <div  
        v-for="disk in disks" 
        :key="disk.author">
        <DiskCard 
        :name="disk.name" 
        :image="disk.poster"  
        :group="disk.author" 
        :year="disk.year" />
        </div>
    </div>
  </section>
</template>

<script>
import axios from 'axios';
import DiskCard from './DiskCard.vue';
export default{
    name: "DisksSection",
    data() {
        return {
            disks: []
        };
    },
    mounted() {
        axios.get("https://flynn.boolean.careers/exercises/api/array/music").then((res) => {
            this.disks = res.data.response;
        });
    },
    components: { DiskCard }
}
</script>

<style>

</style>