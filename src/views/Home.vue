<template>
  <div class="home">
    <NavBar/>
    <BannerOne/>
    <BannerTwo/>
    <BannerThree/>
    <BannerFour/>
    <TheService/>
    <TheFaq/>
    <TheFooter/>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import BannerOne from '@/components/BannerOne.vue'
import BannerTwo from '@/components/BannerTwo.vue'
import BannerThree from '@/components/BannerThree.vue'
import BannerFour from '@/components/BannerFour.vue'
import TheService from '@/components/TheService.vue'
import TheFaq from '@/components/TheFaq.vue'
import TheFooter from '@/components/TheFooter.vue'

export default {
  name: 'Home',

  components: {
    NavBar,
    BannerOne,
    BannerTwo,
    BannerThree,
    BannerFour,
    TheService,
    TheFaq,
    TheFooter
  }
}
</script>
