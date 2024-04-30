<template>
  <!-- <RouterView/> -->
  <Home />
  <Filters />
  <Pagination />
  <keepExploring />
  <startBuying />
  <footers />
</template>

<script>
import Home from './components/Home.vue'
import Filters from './components/filters.vue'
import Pagination from './components/pagination.vue'
import keepExploring from './components/keepExploring.vue'
import startBuying from './components/startBuying.vue'
import footers from './components/footers.vue'

export default {
  name: 'App',
  components: {
    Home, Filters, Pagination, keepExploring, startBuying, footers
  }
}
</script>

<style></style>
