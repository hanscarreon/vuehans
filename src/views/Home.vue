<template>
  <div class="" id="home">
    <BannerHome/>
    <Service/>
    <Products/>
    <Partner/>
    <News/>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/Banner.vue'
import BannerHome from '@/components/BannerHome.vue'
import Service from '@/views/Service.vue'
import Products from '@/views/Products.vue'
import Partner from '@/views/Partner.vue'
import News from '@/views/News.vue'

export default {
  name: 'Home',
  components: {
    Service,
    BannerHome,
    Products,
    Partner,
    News

  }
}
</script>


