<template>
  <div class="home">
  	<CallToAction/>
    <HospitalSearch/>
    <SearchResults/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import HospitalSearch from '@/components/HospitalSearch.vue' // @ is an alias to /src
import CallToAction from '@/components/CallToAction.vue'
import SearchResults from '@/components/SearchResults.vue'

export default Vue.extend({
  name: 'home',
  components: {
  	CallToAction,
    HospitalSearch,
    SearchResults
  }
})
</script>
