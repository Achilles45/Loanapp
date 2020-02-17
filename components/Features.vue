<template>
  <section class="features">
      <div class="container">
          <div class="row">
              <div class="col-12 text-center">
                  <h3>Why You Should Use LoanApp?</h3>
              </div>
          </div>
          <div class="why__wrapper">
              <div class="why__card">
                  <div class="image">
                      <img src="../assets/images/half-maze-gray.png" class="img" alt="">
                  </div>
                  <h5>Speed & Efficiency</h5>
                  <p>Speed and efficiency is at the base of all we do. We respond to all your request as soon as we get them. There is no need to wait for hours for feedback.</p>
              </div>
               <div class="why__card">
                    <div class="image">
                      <img src="../assets/images/half-maze-green.png" class="img" alt="">
                  </div>
                  <h5>Security</h5>
                  <p>Your privacy and security is very important to us. We make sure all your details are properlly encrypted and are safe at all times.</p>
              </div>
               <div class="why__card">
                    <div class="image">
                      <img src="../assets/images/half-maze-orange.png" class="img" alt="">
                  </div>
                  <h5>24/7 Support</h5>
                  <p>We have a top notch customer support team that are literally available to respond to all your queries at any time as we believe that our customers are key to our success.</p>
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
.features{
    background: #F6F7FF;
    padding: 4rem 0;
    h3{
        color: #454545;
        font-weight: bold;
    }
    .why__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        grid-gap: 30px;
        margin-top: 2rem;
        .why__card{
            background: #fff;
            padding: 4rem 2rem;
            position: relative;
            .image{
                position: absolute;
                bottom: 0;
                right: 0;
                .img{
                    max-width: 100px;
                    height: auto;
                }
            }
            h5{
                padding-bottom: 2rem;
                color: #454545;
                font-weight: 400;
                text-transform: uppercase;
                font-size: 1rem;
            }
            p{
                font-size: .9rem;
                padding-bottom: 2rem;
                color: #545454;
                line-height: 1.7;
            }
        }
    }
}
</style>