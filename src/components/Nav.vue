<template>
   

<div id="nav-main" class="container">
    <nav class="navbar navbar-expand-md navbar-light bg-white">
        <router-link  to="/" class="navbar-brand"><img src="../assets/img/logopci.png" class="d-inline-block align-top" height="auto" width="150px" alt=""></router-link>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav mr-auto">
            <!-- /. spacer -->
            </ul>
            <ul class="navbar-nav">
                <li class="nav-item m-2">
                    <router-link class="nav-link" to="/about">ABOUT</router-link>
                </li>
                <li class="nav-item m-2">
                    <router-link class="nav-link" to="/service">WHAT WE DO</router-link>
                </li>
                <li class="nav-item m-2">
                    <router-link class="nav-link" to="/news">NEWS</router-link>
                </li>
                <li class="nav-item m-2">
                    <router-link class="nav-link" to="/contact">CONTACT US</router-link>
                </li>
            </ul>
        </div>
    </nav>
    
</div>


      
</template>

<script>
export default {
  name: 'navbar'
}
</script>

<style scope lang="scss">
@import "../style/_variables.scss";

.nav-bg{
    background-color: $color-white;
}
.router-link-active{
    color: $color-green!important;
}
#navbarNav{
    .navbar-nav{
        .nav-item{
            font-family: 'sta-reg';
            font-size: 1.5em;
            a{
                color : $color-black;
            }
        }
        
    }
}

</style>