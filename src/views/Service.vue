<template>

<div class=" mt-5 container-lg" id="services">
        <div class="row">
         <div class="col-12"> <h1 class="header-title">Our services<span class="color-green">.</span> </h1></div>
          <div class="col-lg-6 col-md-6 col-sm-12 col-12 service-holder">
            <img class="rounded-circle" src="@/assets/services/vr_2.png" alt="Generic placeholder image" width="140" height="140">
            <h2 class=" header-services">VIRTUAL REALITY PLATFORMS</h2>
            <p class="text-justify">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna.</p>
            <p><a class="btn btn-green text-white" href="#" role="button">Go to website »</a></p>
          </div><!-- /.col-lg-4 -->
          <div class="col-lg-6 col-md-6 col-sm-12 col-12 service-holder">
            <img class="rounded-circle" src="@/assets/services/lms.png" alt="Generic placeholder image" width="140" height="140">
            <h2 class="header-services">Heading</h2>
            <p class="text-justify">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna.</p>
            <p><a class="btn btn-green text-white" href="#" role="button">Go to website »</a></p>
          </div><!-- /.col-lg-4 -->
        </div>
    </div>
    
</template>

<script>
import axios from 'axios'
import VueAxios from 'vue-axios'

export default {
    name:'service'
}
</script>

<style  scoped lang="scss">
@import "../style/_variables.scss";
#services{
  .header-title{
    font-family: 'sta-reg';
    text-transform: uppercase;
  }
  .btn-green{
    background-color: $color-green;
    border-radius: 15px;
  }
  .header-services{
    font-family: 'sugo-trial';
    color: $color-orange;
  }
  .service-holder{
    padding: 0 125px;
    p{
        font-family: 'lt-light';
    }
  }
}


@media screen and (max-width: $breakpoint-tablet) {
   .service-holder{
    padding: 0 50px!important;
  }
  
}

@media screen and (max-width: $breakpoint-mobile) {
   .service-holder{
    padding: 0 30px!important;
  }
  
}
    
    

</style>