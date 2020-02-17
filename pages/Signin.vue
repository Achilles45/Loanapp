<template>
  <section class="register">
      <div class="container">
         <div class="row pt-3">
             <div class="col-md-3"></div>
             <div class="col-md-6 pt-5">
                 <h3 class="text-center">Welcome Back!</h3>
                 <p class="text-center">Login to continue. </p>
                 <div class="row">
                     <div class="col-12">
                         <form action="">
                            <div class="form-group">
                                <label for="email">Email Adress</label>
                                <input type="text" class="form-control" v-model="email" placeholder="smithwilliams@gmail.com">
                            </div>
                             <div class="form-group">
                                <label for="email">Password</label>
                                <input type="password" class="form-control" v-model="password" placeholder="************">
                            </div>
                            
                             <small>By clicking sign in, you agree to our terms and conditions.</small><br><br>
                             <button type="submit" class="signin__btn">Sign In</button>
                             <div class="bottom text-center">
                                 <p class="bottom-p">Yet to have an account? <nuxt-link to="register">Create Account</nuxt-link></p>
                             </div>
                         </form>
                     </div>
                 </div>
             </div>
             <div class="col-md-3"></div>
         </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.register{
    background: #251F68;
    // height: 100vh;
    display: flex;
    justify-content: center;
    align-content: center;
    // padding: 4rem 0;
    h3{
        color: #fff;
    }
    p{
        color: #fff;
        padding-bottom: 1rem;
        opacity: .8;
        font-size: .9rem;
    }
    form{
        background: #f7f7f7;
        padding: 3rem 2rem;
        border-radius: 4px;
        margin-bottom: 3rem;
       label{
           color: #454545;
           font-size: .8rem;
           font-weight: bold;
           opacity: .8;
       }
       input{
           font-size: .8rem;
           height: 2.8rem;
           box-shadow: none;
           color:#545454;
       }
       small{
           color: #627071;
       }
       .signin__btn{
           background: #251F68;
           width: 100%;
           padding: 1rem 3rem;
           border-radius: 3px;
           text-decoration: none;
           color: #fff;
           border: none;
           font-size: .8rem;
           &:hover{
               background: #33B27B;
               transition: all ease-in-out .5s;
           }
       }
       .bottom-p{
           color: #454545;
           padding-top: 2rem;
           a{
               color: #251F68;
               font-size: .8rem;
               font-weight: bold;
           }
       }
    }
}
</style>