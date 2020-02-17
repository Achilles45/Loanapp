<template>
  <section class="app">
      <div class="container">
          <div class="row">
              <div class="col-md-1"></div>
              <div class="col-md-10">
                  <div class="app__wrapper text-center">
                     <p>Sometimes a life line is what you need to stay alive in business and we are here to provide that to you at a very cheap rate.</p>
                     <nuxt-link to="/register" class="register__btn">Get Started Now</nuxt-link>
                  </div>
              </div>
              <div class="col-md-1"></div>
          </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.app{
    background: #fff;
    padding: 7rem 0;
    .app__wrapper{
        background: #251F68;
        padding: 5.5rem 3rem;
        border-radius: 10px;
        color: #fff;
        p{
            padding-bottom: 3rem;
            line-height: 1.6;
            opacity: .8;
        }
        .register__btn{
            border: 1px solid #fff;
            border-radius: 4px;
            text-decoration: none;
            padding: 1.2rem 3rem;
            color: #fff;
            font-size: .8rem;
            &:hover{
                padding: 1.2rem 4rem;
                transition: all ease-in-out .5s;
            }
        }
    }
}
</style>