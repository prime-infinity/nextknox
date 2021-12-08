<template>
    <div class="row pt-4 pt-md-0 bg-main" style="height:100vh;">

        <div class="col-12 my-auto">

            <div class="row pt-4">
                <div class="col-11 col-md-5 mx-auto">

                 
                    <form @submit.prevent="loginUser">

                        <div class="form-group mb-4 pb-2">
                            <input v-model="userData.acctNun" class="form-control custom-input" id="exampleInputEmail1" placeholder="Enter Account Number">
                        </div>

                        <div class="form-group mb-4 pb-2">
                            <input v-model="userData.password" type="password" class="form-control custom-input" placeholder="Enter Password" id="exampleInputPassword1">
                            <small v-if="errors.password" class="text-danger">{{ errors.password }}</small>
                        </div>
                        
                        <div class="form-group mb-4 pb-2">
                            <input v-model="userData.password_confirmation" type="password" class="form-control custom-input" id="exampleInputPasswordConfirm1" Placeholder="Confirm password">
                        </div>

                        <button :disabled="loggin" type="submit" class="btn btn-custom pt-3 pb-3 font-weight-bold">
                            <div v-show="!loggin">Sign Up</div>
                            <span v-show="loggin" class="spinner-border spinner-border-sm" role="status" aria-hidden="true"></span>
                        </button>

                        
                   
                        <div class="text-center mt-5">
                            Already a member <router-link to="/login"><a>Sign In</a></router-link>
                        </div>
  
                    </form>
                </div>
            </div>
            
        </div>

    </div>
</template>

<script>
    export default {
        name: 'register',
        data(){
            return{
                userData:{
                    acctNun:'',
                    password:'',
                    password_confirmation:'',
                },
                errors:{},
                loggin:false,
            }  
        },    
           computed:{

        }, 
        methods: {
            loginUser:function(){
                this.$router.push('home')
            }
        },  
    }
</script>

<style>
  
</style>