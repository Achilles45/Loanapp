<template>
 <div class="contact">
     <Navbar />
     <div class="contact__wrapper">
        <div class="container">
            <h3 class="text-right">Contact Us</h3>
        </div>
     </div>
     <div class="container">
         <div class="row contact__body pt-5">
             <div class="col-md-7 pt-5">
                 <h5>Reach out to us today!</h5>
                 <p>The support team is always ready to respond to all your queries</p><br>
                 <div v-if="err" class="alert alert-danger">
                     {{ err }}
                 </div>
                  <div v-if="success" class="alert alert-success">
                     {{ success }}
                 </div>
                 <form action="" @submit.prevent="sendMessage()">
                     <div class="row">
                         <div class="col-md-6">
                             <div class="form-group">
                                 <input type="text" class="form-control" placeholder="What's your name" v-model="name">
                             </div>
                         </div>
                          <div class="col-md-6">
                             <div class="form-group">
                                 <input type="email" class="form-control" placeholder="What's is your email address" v-model="email">
                             </div>
                         </div>
                     </div>
                     <div class="row">
                         <div class="col-12">
                             <textarea name="" id="" cols="80" rows="7" class="form-control" v-model="message" placeholder="Tell us your message here"></textarea>
                         </div>
                     </div><br>
                     <button type="submit" class="form__btn">Send Message</button>
                 </form>
             </div>
             <div class="col-md-2"></div>
             <div class="col-md-3 body">
                 <p>You can also reach out to us through email or come visit the office</p><br>
                 <h5>Office Address</h5>
                 <p>245 East Ohio Street, Chicago, IL 60611 </p>
                 <h5>Email Address</h5>
                 <p>example@gmail.com </p>
                 <h5>Phone Number</h5>
                 <p>+1 618-710-6254</p>
             </div>
         </div>
     </div><br><br>
      <hr />
     <Footer />
 </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Footer from '~/components/Footer.vue'
import db from '~/firebase/init'
export default {
    data(){
        return{
            name:null,
            email:null,
            message:null,
            err:null,
            success:null,
        }
    },
    components:{
        Navbar,
        Footer
    },
    methods:{
        sendMessage(){
            if(!this.name || !this.email || !this.message){
                this.err = 'Fields cannot be empty, please try again!'
                this.removeAlert();
            }else{
                db.firestore().collection('messages').add({
                    name:this.name,
                    email:this.email,
                    message:this.message
                })
                this.success = 'Message successful sent. We will get back to you shortly!'
                this.name = '';
                this.email = '';
                this.message = '';
                this.removeAlert();
            }
        },
        removeAlert(){
            setTimeout(() => {
                document.querySelector('.alert').remove()
            }, 3000);
        }
    }
}
</script>

<style lang="scss" scoped>
.contact__wrapper{
     background: linear-gradient(rgba(37,31,104,.9), rgba(37,31,104,.9)), url('../assets/images/city.jpeg');
    padding: 6rem 0;
    color: #fff;
    h3{
        padding-top: 5rem;
        font-weight: bold;
    }
}
.contact__body{
    h5{
        color: #454545;
        font-size: 1.2rem;
    }
    p{
        color: #545454;
        font-size: .9rem;
        opacity: .9;
    }
    form{
        input{
            height: 2.8rem;
            border-radius: 0px;
            box-shadow: none;
            font-size: .8rem;
        }
        textarea{
            border-radius: 0px;
            box-shadow: none;
            font-size: .8rem;
        }
        .form__btn{
            background: #251F68;
            color: #fff;
            text-decoration: none;
            padding: .8rem 3rem;
            border-radius: 4px;
            border: none;
            font-size: .8rem
        }
    }
}
.body{
    h5{
        font-size: .9rem;
        opacity: .9;
        color: #454545;
    }
    p{
        font-size: .8rem;
        opacity: .9rem;
        color: #545454;
    }
}
.alert{
    font-size: .9rem;
}
</style>