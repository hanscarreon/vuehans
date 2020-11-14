<template>
  <div class="news">
     <div class="container">
       <div class="row">
         <div class="col-md-12 col-sm-12">
           <!-- <VueSlickCarousel  v-bind="settings">
                <div v-for="data in info" v-bind:key="data.id" class="holder-slick" >
                  <img height="auto" img="100%" :src=" require(`@/assets/img/${data.img}`)" />
             </div>
          </VueSlickCarousel> -->
         </div>
       </div>
     </div>
  </div>
</template>

<script>
import NewsFile from '../assets/json/news.json'
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
export default {
    name: 'news',
    data () {
      return {
        info: null,
         settings: {
          centerMode: true,
          centerPadding: "20px",
          focusOnSelect: true,
          infinite: true,
          slidesToShow: 3,
          speed: 500

        }
        
      }
    },
    components: { VueSlickCarousel },
    mounted(){
        this.info = NewsFile.news ;
        console.log(NewsFile.news)

    }
   
}
</script>


<style lang="scss" scoped>
@import "../style/_variables.scss";
#news{

}

</style>
