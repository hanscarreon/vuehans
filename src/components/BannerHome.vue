<template>
    <div id="banner">
        <div class="container">
          <div class="row">
             <div class="col-md-6 col-sm-12 col-12 ">
                <h1 class="banner-title">SIMPLIFY LEARNING</h1>
                <p class="banner-desc text-left">PCI Tech Center is an organization that aims to bring excellent, interactive, and immersive learning to every corner of the country with new and engaging technologies.</p>
            </div>
          </div>
        </div>
      </div>
</template>

<script>
export default {
    name : 'bannerhome'
}
</script>
<style scoped lang="scss">
@import '../style/_variables.scss';

#banner{
  background:url('../assets/img/bg_1.png');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center ;
  padding: 50px 0;
  .banner-title{
    font-family: 'ft-bold';
    color: $color-green;
    .banner-desc{
      font-family: 'ft-book';
    }
  }
    
}


</style>