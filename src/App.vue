<template>
  <div id="app">
    
    <keep-alive>
      <router-view></router-view>
    </keep-alive>

    <app-tabs/>

  </div>
</template>

<script>
import Tabs from './components/Tabs.vue'
export default {
  components: {
    [Tabs.name]: Tabs
  }
}
</script>

<style>

</style>
