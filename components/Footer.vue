<template>
  <footer class="container-fluid">
      <div class="container">
          <div class="row">
              <div class="col-md-4">
                  <h5>Company</h5>
                  <p>LoanApp is a consumer focused fintech that aims to bridge the gap of poor access to finance. We believe that a little support to our customers will go a long way into boosting productivity thus producing wealth. More features will roll out soon to serve our customers better.</p>
              </div>
              <div class="col-md-4">
                  <h5>Contact Details</h5>
                  <h6>Head Office</h6>
                  <p>30 Omotayo Ojo Street, Off Allen Aenue, Ikeja, Lagos State, Nigeria.</p>
                  <h6>Email Address</h6>
                  <p>example@gmai.com</p>
                  <h6>Phone</h6>
                  <p>+2348 102 365 365</p>
              </div>
              <div class="col-md-4">
                  <h5>Disclaimer</h5>
                  <p>LoanApp is a complete paperless company that does not drive any form of business through agents networks. Please kindly know that LoanApp will not help responsible for a transaction carried out through physical agents as we do not have agents anywhere in the world.</p>
              </div>
          </div>
          <hr>
          <p>&copy; All right reserved. LoanApp. 2020. <nuxt-link to="/">terms and conditions apply.</nuxt-link></p>
      </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
footer{
    padding: 5rem 0;
    h5{
        padding-bottom: 2.5rem;
        font-size: 1rem;
        color: #454545;
        font-weight: bold;
        opacity: .8;
    }
   h6{
       color: #454545;
       font-size: .9rem;
       font-weight: 400;
   }
   p{
       color: #545454;
       font-size: .84rem;
       opacity: .8;
       line-height: 1.6;
   }
}
</style>