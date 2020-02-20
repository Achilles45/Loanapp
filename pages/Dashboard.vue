<template>
  <div class="dashboard">
      <div class="left">
          <div class="heading">
              <h4>Welcome Back</h4>
                <small>{{ email }}</small><br /><br />
                <ul class="pt-4">
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'database']"/>&nbsp; Dashboard</nuxt-link></li><hr />
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'users']"/>&nbsp; Profile</nuxt-link></li><hr />
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'shopping-cart']"/>&nbsp; Balance</nuxt-link></li><hr />
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'cogs']"/>&nbsp; Request Loan</nuxt-link></li><hr />
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'clone']"/>&nbsp; Make Withdrawal</nuxt-link></li><hr />
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'cubes']"/>&nbsp; Invest</nuxt-link></li><hr />
                    <li><nuxt-link to="/"><font-awesome-icon :icon="['fa', 'sign-in']"/>&nbsp; Logout</nuxt-link></li><hr />
                </ul>
          </div>
      </div>
      <div class="right">
          <div class="heading">
              <h3>Hey Achilles</h3>
              <p>We are glad to have you back. Have a nice time using our platform</p>
          </div>
          <hr>
           <div class="right__content">
              <small>Look at the summary of your activities here</small>
              <div class="right__wrapper">
                  <div class="right__card card__1 d-flex">
                     <div class="icon pr-3">
                          <font-awesome-icon :icon="['fa', 'shopping-cart']"/>
                     </div>
                      <div class="text">
                          <h6>Wallet Balance</h6>
                          <p>$00.00</p>
                      </div>
                  </div>
                  <div class="right__card card__2">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, voluptatum!
                  </div>
                  <div class="right__card card__3">
                      Lorem ipsum dolor sit amet consectetur adipisicing elit. Error, voluptatum!
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
import firebase from 'firebase';
export default {

}
</script>

<style lang="scss" scoped>
.dashboard{
    display: grid;
    grid-template-columns: 300px 1fr;
    height: 100vh;
    .left{
        background: #251F68;
        padding: 3rem 3rem;
        color: #fff;
        ul li a{
            color: #fff;
            opacity: 0.8;
            font-size: .82rem;
            text-decoration: none;
        }
    }
    .right{
        background: #fafafa;
        padding: 3rem 2rem;
        .heading{
            h3{
                color: #2b2b2b;
                font-size: 1rem;
            }
            p{
                font-size: .85rem;
                color: #2b2b2b;
                opacity: .9;
            }
        }
        .right__content{
            .right__wrapper{
                display: grid;
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
                grid-gap: 25px;
                margin-top: 2rem;
                .right__card{
                    padding: 1rem 2rem;
                    color: #fff;
                    border-radius: 4px;
                    font-size: .8rem;
                    h6{
                        font-size: .8rem;
                    }
                    p{
                        font-size: .9rem;
                    }
                }
                .card__1{
                    background: #ff808b;
                }
                .card__2{
                    background: #757afc;
                }
                .card__3{
                    background: #0facf3;
                }
            }
        }
    }
}
</style>