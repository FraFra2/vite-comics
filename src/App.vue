<script>
import headerApp from './components/headerApp.vue'
import bodyApp from './components/bodyApp.vue'
import mainNavApp from './components/mainNavApp.vue'
import footerApp from './components/footerApp.vue'

export default{
  components: {
    headerApp,
    bodyApp,
    mainNavApp,
    footerApp
  }
}

</script>


<template> 
  
  <div class = "h-screen">
    <headerApp class = "container mx-auto"/>

    <bodyApp/>

    <mainNavApp/>
    
    <footerApp/>
  </div>

</template>

<style>
*{
  font-family: 'Encode Sans Condensed', sans-serif;
}
</style>
