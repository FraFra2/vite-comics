<script>
export default {
  data() {
    return {
      navLinks: [
        {
          label: "digital comics",
          icon: "src/assets/buy-comics-digital-comics.png"
        },
        {
          label: "dc merchandise",
          icon: "src/assets/buy-comics-merchandise.png"
        },
        {
          label: "subscription",
          icon: "src/assets/buy-comics-subscriptions.png"
        },
        {
          label: "comic shop locator",
          icon: "src/assets/buy-comics-shop-locator.png"
        },
        {
          label: "dc power visa",
          icon: "src/assets/buy-dc-power-visa.svg"
        },
      ]
    }
  }
}
</script>

<template>
  <div class="
            bg-[#0082f9] text-white">
    <div class = "
                  flex gap-8 items-center
                  py-8
                  w-[70%]
                  mx-auto
                  ">
      <div v-for = "(item, i) in navLinks" :key = "item.label">
          <div class = "flex items-center">
            <img 
            :src= "item.icon" 
            :alt = "item.label"
            class = "w-[30px]">
            <span class = "uppercase ml-4">
              {{ item.label }}
            </span>
          </div>
      </div>
   </div>
  </div>
</template>

<style scoped>



</style>