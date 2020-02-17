<template>
  <div class="about__wrapper">
      <Navbar />
      <div class="about__heading">
          <div class="container">
              <h3 class="text-right">About us</h3>
          </div>
      </div>
      <div class="about__body">
          <div class="row">
              <div class="col-md-2"></div>
              <div class="col-md-8"></div>
              <div class="col-md-2"></div>
          </div>
      </div>
      <Footer />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'
export default {
    components:{
        Navbar,
        Footer
    }
}
</script>

<style lang="scss" scoped>
.about__heading{
    background: linear-gradient(rgba(37,31,104,.9), rgba(37,31,104,.9)), url('../assets/images/city.jpeg');
    padding: 6rem 0;
    color: #fff;
    h3{
        padding-top: 5rem;
        font-weight: bold;
    }
}
</style>