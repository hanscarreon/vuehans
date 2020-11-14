<template>

<div id="topbar" class="">
    <div class="container">
        <div class="row" >
            <div class="col-md-6 col-sm-12" id="op-text">
                <h5 class="mt-2">Opening hours 8:00 am - 6:00 pm</h5>
            </div>
            <div id="icon-holder" class="col-md-6 col-sm-12">
            <a class="icon-bg btn"><i class="fab fa-facebook-f icon-color"></i></a>
            <a class="icon-bg btn"><i class="fab fa-twitter icon-color"></i></a>
            <a class="icon-bg btn"><i class="fab fa-instagram icon-color"></i></a>
            </div>
        </div>
    </div>
</div>
    
</template>

<script>
export default {
    name:'topbar'
}
</script>

<style  scoped lang="scss">
@import "../style/_variables.scss";
#topbar{
    background-color: $color-green;
    h5{
        color: $color-white;
        font-family: 'lt-light';
    }
    #op-text{
        text-align: left;
    }
     #icon-holder{
        text-align: right;
            .icon-color{
                color: $color-white;
                font-size:1.5em ;
            }
    }

   
}


@media screen and (max-width: $breakpoint-websmall) {
    #icon-holder{
        text-align: center!important;
    }
    #op-text{
        text-align: center!important;
    }
  
}
    

</style>