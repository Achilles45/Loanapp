<template>
  <div class="navbar">
       <div class="navbar__contents container d-flex justify-content-between align-items-center">
        <div class="hero__logo">
            <h3><nuxt-link to="/" class="logo">LoanApp</nuxt-link></h3>
        </div>
        <ul class="d-flex justify-conetent-between pt-2">
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/about">About Us</nuxt-link></li>
            <li><nuxt-link to="/">Products</nuxt-link></li>
            <li><nuxt-link to="/">Contact Us</nuxt-link></li>
            <li><nuxt-link to="/register">Create a free account</nuxt-link></li>
            <li><nuxt-link to="/signin" class="login__link">Sign In</nuxt-link></li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
 .navbar{
padding-top: 2rem;
color: #fff;
background: #fff !important;
position: fixed;
z-index: 1000;
width: 100%;
box-shadow: 3px 0px 5px rgba(0,0,0,.15);
.logo{
    font-weight: bold;
    text-decoration: none;
    color: #251F68;
}
ul{
    li a{
        color: #545454;
        font-size: .8rem;
        margin: 0 .7rem;
        font-weight: bold;
        opacity: .9;
        text-decoration: none;
        text-transform: uppercase;
    }
    .login__link{
        background: #251F68;
        padding: 1.2rem 3rem;
        border-radius: 3px;
        color: #fff;
        opacity: 1 !important;
        &:hover{
            background: #33B27B;
            transition: all ease-in .5s;
        }
    }
}
    }
</style>