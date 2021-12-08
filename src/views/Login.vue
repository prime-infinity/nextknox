<template>
    <div class="row pt-4 pt-md-0 bg-main" style="height:100vh;">

        <div class="col-12 my-auto">

            <div class="row pt-4">
                <div class="col-11 col-md-5 mx-auto">

                    <form @submit.prevent="loginUser">
                    
                        <div class="form-group mb-4 pb-2">
                            <input v-model="userData.acctNun" class="form-control custom-input" id="exampleInputEmail1" placeholder="Enter Account Number">
                        </div>

                        <div class="form-group mb-4 pb-3">
                            <input v-model="userData.password" type="password" class="form-control custom-input" placeholder="Enter Password" id="exampleInputPassword1">
                            <small v-if="errors.password" class="text-danger">{{ errors.password }}</small>
                        </div>

                        <button :disabled="loggin" type="submit" class="btn btn-custom pt-3 pb-3 font-weight-bold">
                            <div v-show="!loggin">Sign in</div>
                            <span v-show="loggin" class="spinner-border spinner-border-sm" role="status" aria-hidden="true"></span>
                        </button>

                        
                   
                        <div class="text-center mt-5">
                            Not yet a member <router-link to="/register"><a>Sign Up</a></router-link>
                        </div>
  
                    </form>
                </div>
            </div>
            
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
            loginUser:function(){
                this.$router.push('home')
            }
        },  
    }
</script>

<style>
    .custom-input{
        border-radius: 100px;
        height:56px;
    }
    .custom-input:focus,
    .custom-input:hover{
        transition:.5s ease;
        
    }
</style>