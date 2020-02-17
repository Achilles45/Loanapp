<template>
  <section class="loan">
     <div class="row">
         <div class="col-12 text-center">
             <h3>You are 3 clicks away from securing a loan</h3>
             <p>The process is simple and can be completed in 3 minutes</p>
         </div>
     </div>
     <div class="process__wrapper container">
         <div class="process__card">
            <img src="../assets/images/register.png" class="process__icons" alt="">
            <h5>Create your Account</h5>
            <p>We are completely paperless in all our operations and within seconds, you are done creating an account.</p>
         </div>
          <div class="process__card">
            <img src="../assets/images/request.png" class="process__icons" alt="">
            <h5>Request for a loan</h5>
            <p>We use machine learning to score you base on your details and so we can calculate how much you qualify for.</p>
         </div>
          <div class="process__card">
            <img src="../assets/images/wallet.png" class="process__icons" alt="">
            <h5>Make withdrawer</h5>
            <p>Once your wallet has been credited, you can then proceed to make withdrawers.</p>
         </div>
     </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.loan{
    padding: 5rem 0;
    h3{
        color: #454545;
        font-weight: bold;
    }
p{
        font-size: .9rem;
        color: #545454;
    }
    .process__wrapper{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
        grid-gap: 30px;
        margin-top: 2rem;
        .process__card{
            // box-shadow: 3px 0px 5px rgba(0,0,0,.15);
            padding: 2rem;
            text-align:center;
            .process__icons{
                max-width: 50px;
                height: auto;
                padding-bottom: 1.5rem;
            }
            h5{
                padding-bottom: .8rem;
                font-weight: 400;
                font-size: 1rem;
                color: #454545;
                border-bottom: 1px solid #ebebeb;
            }
            p{
                font-size: .9rem;
                color: #545454;
                line-height: 1.7;
                font-weight: 400;
            }
        }
    }
}
</style>