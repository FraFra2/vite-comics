<script>
export default {
  data() {
    return {
      navLinks:[
        {
            label: "Characters",
            ref: "#"
        },
        {
            label: "Comics",
            ref: "#"
        },
        {
            label: "Movies",
            ref: "#"
        },
        {
            label: "TV",
            ref: "#"
        },
        {
            label: "Games",
            ref: "#"
        },
        {
            label: "Collectibles",
            ref: "#"
        },
        {
            label: "Videos",
            ref: "#"
        },
        {
            label: "Fans",
            ref: "#"
        },
        {
            label: "News",
            ref: "#"
        },
        {
            label: "Shop",
            ref: "#"
        },
      ]
    }
  }
}
</script>

<template>
        <header class = "py-6 w-[70%] mx-auto flex justify-between items-center">
            <div class = "logo-cont">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            <div class = "nav-cont">

                <ul class = "
                            flex gap-4
                            ">
                    <li v-for="(link, i) in navLinks"
                        class = "
                                uppercase
                                hover:text-[#0082f9] hover:underline
                                decoration-8
                                underline-offset-[61px]
                                ">
                        <a :href = "link.ref" >{{link.label}}</a>
                    </li>
                </ul>

            </div>
        </header>
        
        <div class = "jumbo h-80 overflow-hidden">
            <img src="src/assets/jumbotron.jpg" class = "overflow-hidden">
        </div>

</template>

<style scoped>

.jumbo {
    
}

</style>