<script>
export default {
  props: {
    thumbNail : String,
    price: String,
    serie: String,
  },
  data() {
    return {
    }
  }
}
</script>

<template>
  <div>
    <img :src="thumbNail" class = "w-[250px] h-[250px]">
    <div class = "flex justify-between">
      <h2 class = "text-lg">
        {{ this.serie }}
      </h2>
      <h2 class = "bg-green-600 p-1 rounded-sm m-1">
        {{ this.price }}
      </h2>
    </div>
    
  </div>
</template>

<style scoped>



</style>