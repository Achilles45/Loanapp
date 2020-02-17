<template>
  <section class="hero">
      <div class="container">
          <!--End of Hero Navbar Section -->
          <!--Banner section -->
          <div class="banner__wrapper">
              <div class="row">
                  <div class="col-md-6">
                      <h1>Need a quick loan for your business?</h1>
                      <p>Loanapp is a financial service provider that provides her customers with quick access to credit for their business, health ands at competitive interest rates.</p>
                      <nuxt-link to="/register" class="banner__btn">Create a free account</nuxt-link>
                  </div>
                  <div class="col-md-6 d-none d-md-block">
                      <img src="../assets/images/img1.png" class="img-fluid img" alt="">
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.hero{
    background: #251F68;
    height: 100vh;
    .banner__wrapper{
        padding-top: 13rem;
        color: #fff;
        h1{
            font-weight: bold;
            padding-bottom: 1.2rem;
            text-transform: capitalize;
            line-height: 1.6;
        }
        p{
            opacity: .7;
            padding-bottom: 3rem;
            font-size: 1rem;
            line-height: 1.8;
        }
        .banner__btn{
          font-size: .9rem !important;
          text-decoration: none;
          background: #33B27B;
          padding: 1.5rem 3.5rem;
          border-radius: 4px;
          color: #fff;
          font-weight: 600;
          &:hover{
              padding: 1.5rem 4.5rem;
              transition: all ease-in-out .5s;
          }
        }
        .img{
            animation-name: animate;
            animation-duration: 2s;
            animation-iteration-count: infinite;
            animation-direction: alternate;
        }
    }
}
//Animation
@keyframes animate{
    from{
        transform: translateY(-10px);
    }
}
</style>