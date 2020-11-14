<template>
    <div id="partner">
        <div class="container mt-4 mb-4">
            <div class="row">
                <div class="partners-header-block col-12 col-sm-12">
                    <h1 class="partners-title">OUR PARTNERS<span class="color-green">.</span></h1>
                </div>
                <div class="col-md-6 col-sm-12 col-12">
                <img width="100%" height="auto" src="../assets/img/bg_2.jpg">
                </div>
                <div class="col-md-6 col-sm-12 col-12">
                        <div class="row" id="partners-logo">
                            <div class="col-md-4 col-sm-6 col-6">
                                <img  class="mt-5" src="../assets/img/p3.png">
                            </div>
                            <div class="col-md-4 col-sm-6 col-6">
                                <img  class="mt-5" src="../assets/img/p2.png">
                            </div>
                            <div class="col-md-4 col-sm-6 col-6">
                                <img  class="mt-5" src="../assets/img/p4.png">
                            </div>
                            <div class="col-md-6 col-sm-6 col-6">
                                <img  class="mt-5" src="../assets/img/p4.png">
                            </div>
                            <div class="col-md-6 col-sm-12 col-12">
                                <img  class="mt-5" src="../assets/img/p7.png">
                            </div>
                        </div>
                    
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'partner'
}
</script>

<style lang="scss" scoped>
@import "../style/_variables.scss";

#partner{
    .partners-title{
         font-family: "sta-reg";
        text-transform: uppercase;
        color: $color-black;
    }
    #partners-logo{
        img{
            height: auto;
            width: 100px;
        }
    }
}


</style>