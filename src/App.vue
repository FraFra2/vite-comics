<script>
import headerApp from './components/headerApp.vue'
import bodyApp from './components/bodyApp.vue'
import mainNavApp from './components/mainNavApp.vue'
export default{
  components: {
    headerApp,
    bodyApp,
    mainNavApp
  }
}

</script>


<template>

  <div class="container mx-auto">
    <headerApp/>
  </div>
  <bodyApp/>
  <mainNavApp/>
  

</template>

<style>
*{
  font-family: 'Encode Sans Condensed', sans-serif;
}
</style>
