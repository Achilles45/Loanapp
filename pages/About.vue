<template>
  <div class="about__wrapper">
      <Navbar />
      <div class="about__heading">
          <div class="container">
              <h3 class="text-right">About us</h3>
          </div>
      </div>
      <div class="about__body">
          <div class="row pt-5 pb-5">
              <div class="col-md-2"></div>
              <div class="col-md-8 text-center pt-3">
                  <p>LoanApp is a consumer focused fintech startup that provides credit scoring and credit to our users. We use technology to optimize for scale and mass market reach. The company is literally revolutionizing access to credit. We belive in creating opportunities for othrs.</p>
              </div>
              <div class="col-md-2"></div>
          </div>
         <div class="container">
              <div class="row">
              <div class="col-12 heading text-center">
                  <h3>Our Core Values</h3>
              </div>
              <div class="row text-center values pt-4 pb-4">
                  <div class="col-md-4">
                      <h5>Transparency</h5>
                      <p>The company believes in honesty and transparency as we want to be your best choice in enjoying financial services.</p>
                  </div>
                   <div class="col-md-4">
                      <h5>Hardwork</h5>
                      <p>The team is highly motivated everyday to give their best in pursuing the visions of the company.</p>
                  </div>
                   <div class="col-md-4">
                      <h5>Customer centric</h5>
                      <p>Every problem of the customer is our customer. We go the extra steps make sure we resolve all your queries while using our services.</p>
                  </div>
              </div>
          </div>
         </div>
         <br><br>
         <hr>
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
.about__body p{
    color: #545454;
    opacity: .9;
    font-size: .9rem;
    line-height: 1.7;
}
.heading h3{
    color: #454545;
    font-size: 1.3rem;
    font-weight: normal
}
.values{
    h5{
        padding-bottom: 1.2rem;
        border-bottom: 1px solid #ebebeb;
        font-size: 1rem;
    }
    p{
        padding-top: 1.5rem;
        font-size: .9rem;
        color: #545454;
        opacity: .93;
        line-height: 1.7;
    }
}
</style>