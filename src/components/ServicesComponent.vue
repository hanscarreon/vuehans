<template>

<div class=" mt-5 container-lg" id="services">
        <div class="row">
         <div class="col-12"> <h3 class="header-title">Our services</h3></div>
          <div class="col-lg-6 col-md-6 col-sm-12 col-12 service-holder">
            <img class="rounded-circle" src="@/assets/services/vr_2.png" alt="Generic placeholder image" width="140" height="140">
            <h2 class=" header-services">VIRTUAL REALITY PLATFORMS</h2>
            <p class=" text-justify">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna.</p>
            <p><a class="btn btn-secondary" href="#" role="button">View details »</a></p>
          </div><!-- /.col-lg-4 -->
          <div class="col-lg-6 col-md-6 col-sm-12 col-12 service-holder">
            <img class="rounded-circle" src="@/assets/services/lms.png" alt="Generic placeholder image" width="140" height="140">
            <h2 class="header-services">Heading</h2>
            <p class=" text-justify">Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Cras mattis consectetur purus sit amet fermentum. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh.</p>
            <p><a class="btn btn-secondary" href="#" role="button">View details »</a></p>
          </div><!-- /.col-lg-4 -->
        </div>
    </div>
    
</template>

<script>
export default {
    name:'servicescomponent'
}
</script>

<style  scoped lang="scss">
@import "../style/_variables.scss";
#services{
  .header-title{
    font-family: 'sta-reg';
    text-transform: uppercase;
  }
  .header-services{
    font-family: 'sugo-trial';
  }
  .service-holder{
    padding: 0 125px;
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