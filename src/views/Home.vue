<template>
  <div class="home">
  	<CallToAction/>
    <HospitalSearch/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import HospitalSearch from '@/components/HospitalSearch.vue' // @ is an alias to /src
import CallToAction from '@/components/CallToAction.vue'

export default Vue.extend({
  name: 'home',
  components: {
  	CallToAction,
    HospitalSearch
  }
})
</script>
