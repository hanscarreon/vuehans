<template>
    <div id="products">
        <div class="container">
                <div class="row" id="prods">
                    <div class="col-12">
                        <h1 class="prod-title mt-5">OUR PRODUCTS</h1>
                    </div>

                    <div v-for="data in info" v-bind:key="data.id" class="col-md-4 col-sm-12 col-12" >
                        <img :src=" require(`@/assets/img/${data.img}`)" />
                            
                        <h3 class="data-title">{{ data.title }}</h3>
                        <p class="data-desc">{{ data.desc }}</p>
                    </div>

                </div>

        </div>
            

    </div>
</template>

<script>
import Vue from 'vue'
import axios from 'axios'
import VueAxios from 'vue-axios'
import productsFile from '../assets/json/products.json'
Vue.use(VueAxios, axios)

export default {
    name:'products',
    data () {
    return {
      info: null
    }
  },
    mounted(){
        this.info = productsFile.products ;
        //  i dont know why the assets type json not working here 
        //  but working in ionic vue axios
        //  sorry for not solving this problem im still in my working hours when doing this thanks
        this.axios.get('./assets/json/products.json')
      .then(res => { 
          this.info = res.data.events
          console.log(res.data.events);
           })
    }
}
</script>
<style scoped lang="scss">
@import "../style/_variables.scss";

#prods{
 background-color:#f4f4f4;
    .prod-title{
        font-family: "sta-reg";
        text-transform: uppercase;
        color: $color-black;

    }
    .data-title{
        color:$color-orange;
        font-family: "sugo-trial";
    }
    .data-desc{
        font-family: 'lt-light';
        padding: 0 50px;
        text-align: justify;
    }
}

@media screen and (max-width: $breakpoint-websmall) {
    #prods{
        .data-desc{
            font-family: 'lt-light';
            padding: 0 20px;
            text-align: justify;
        }
    }
  
}


</style>