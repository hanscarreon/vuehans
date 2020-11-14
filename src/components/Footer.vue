<template>
    <div id="footer" >
        <div class=" container">
            <div class="row">
                <div class="col-md-6 col-sm-12" id="op-text">
                 <h5 class="mt-2">Copyright @ PCI Innovations Tech Center, Inc. | All rights reserved.</h5>
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



<style  scoped lang="scss">
@import "../style/_variables.scss";
#footer{
    background-color: $color-green;
    h5{
        color: $color-white;
        font-family: 'lt-light';
        font-size: 1em;
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