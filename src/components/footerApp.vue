<script>
import footerBarApp from './footerBarApp.vue'

export default {
  data() {
    return {
      dcComics : [
        "Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"
      ],
      dcShop: [
        "Shop DC",
        "Shop DC Collectibles"
      ],
      dc: [
        "Terms of use", "Privacy Policy(New)", "Ad Choices", "Advertising", "Jobs",
        "Subscription", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help",
        "Contact Us"
      ],
      dcSites: [
        "DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"
      ]
    }
  },
  components: {
        footerBarApp
  },
  
}
components: {

}
</script>

<template>
        <footer class = "text-white">
            <div class="foot-container mx-auto 
                        py-8 w-[70%]">
              <div class = "flex gap-4 columns-3">

                <!-- COL 1 -->
                <div>
                  <h2>
                    DC COMICS
                  </h2>
                  <ul>
                    <template v-for="item in dcComics" :key="item">
                      <li>
                        {{ item }}
                      </li>
                    </template>
                  </ul>

                  <h2>
                    SHOP
                  </h2>
                  <ul>
                    <template v-for="item in dcShop" :key="item">
                      <li>
                        {{ item }}
                      </li>
                    </template>
                  </ul>
                </div>

                <!-- COL 2 -->
                <div>
                  <h2>
                    DC
                  </h2>
                  <ul>
                    <template v-for="item in dc" :key="item">
                      <li>
                        {{ item }}
                      </li>
                    </template>
                  </ul>
                </div>

                <!-- COL 3 -->
                <div>
                  <h2>
                    SITES
                  </h2>
                  <ul>
                    <template v-for="item in dcSites" :key="item">
                      <li>
                        {{ item }}
                      </li>
                    </template>
                  </ul>
                </div>
              </div>
            </div>
        </footer>
        <footerBarApp/>
</template>

<style scoped>
footer{
  background-image: url("src/assets/footer-bg.jpg");
}
footer .foot-container{
  background-image: url("src/assets/dc-logo-bg.png");
  background-repeat: no-repeat;
  background-position: right;

}
h2{
  font-weight: bold;
  font-size: 1.5rem;
}
ul{
  list-style: none;
}
li{
  color: lightgray;
  font-size: .75rem;
}



</style>