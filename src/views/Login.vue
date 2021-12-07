<template>
    <div class="row pt-4 pt-md-0 bg-main text-white">

        <div class="col-12 col-md-7 pt-4">

            <div class="row pt-4">
                <div class="col-11 col-md-8 col-lg-6 mx-auto">

                    <div class="auth-header">
                        <h2 class="font-weight-bold text-center">Sign In</h2>
                    </div>

                    <form @submit.prevent="loginUser">
                    
                        <div class="form-group mb-4">
                            <input v-model="userData.acctNun" type="email" class="form-control customInput" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter Email Address">
                        </div>

                        <div class="form-group mb-4">
                            <input v-model="userData.password" type="password" class="form-control customInput" placeholder="Enter Password" id="exampleInputPassword1">
                            <small v-if="errors.password" class="text-danger">{{ errors.password }}</small>
                        </div>

                        <button :disabled="loggin" type="submit" class="btn btn-blue text-white">
                            <div v-show="!loggin">Sign in</div>
                            <span v-show="loggin" class="spinner-border spinner-border-sm" role="status" aria-hidden="true"></span>
                        </button>

                        <hr class="divider">
                   
                        <div class="text-center mt-4">
                            Not yet a member <router-link to="register"><a href="#">Sign Up</a></router-link>
                        </div>
  
                    </form>
                </div>
            </div>
            
        </div>

        <div class="col-12 col-md-5 d-none d-md-block" id="redleft">

        </div>
    </div>
</template>

<script>
    export default {
        name: 'Login',
        data(){
            return{
                userData:{
                    email:'',
                    acctNun:'',
                },
                errors:{},
                loggin:false,
            }  
        },    
           computed:{

        }, 
        methods: {
            
        },  
    }
</script>
