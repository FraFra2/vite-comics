<script>
export default {
  data() {
    return {
      // Fb, twitter, yt, pinterest, periscope
      socials: [
        {
          label: "Facebook",
          logo: "src/assets/footer-facebook.png"
        },
        {
          label: "Twitter",
          logo: "src/assets/footer-twitter.png"
        },
        {
          label: "YouTube",
          logo: "src/assets/footer-youtube.png"
        },
        {
          label: "Pinterest",
          logo: "src/assets/footer-pinterest.png"
        },
        {
          label: "Periscope",
          logo: "src/assets/footer-periscope.png"
        }
      ]
    }
  }
}
</script>

<template>
  <div class = "bg-[#303030]">
    <div class = "
    w-[70%] mx-auto
    py-6
    flex justify-between items-center">
    <!-- Button -->
      <div>
        <button class = "
        uppercase
      text-white border border-[#0082f9] px-3 py-2">
          sign-up now!
        </button>
      </div>
    <!-- Social -->
      <div class = "flex">
        <h2 class = "
        uppercase
        pr-4
        text-[#0082f9]
        font-bold">
          follow us
        </h2>
        <ul class = "list-none flex items-center gap-4">
          <li v-for="social in socials" :key = "social.label">
            <img :src="social.logo" :alt="social.label">
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>



</style>