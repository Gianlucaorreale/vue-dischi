<template>
  <div>
     <BasesHeader heading ="SPOTIFY"/>
     <DisksSection/>
  </div>
  
</template>

<script>

import BasesHeader from './components/BaseHeader.vue';
import DisksSection from './components/DisksSection.vue'
export default {
  name: 'App',
  components: {
  BasesHeader,
  DisksSection
  }
  
}
</script>

<style lang="scss">
@import './assets/scss/style.scss'  
</style>
