<template>

    <div>
        <div class="row bg-main pb-5">
            
            <div class="col-12 col-md-3 offset-md-1 text-white text-center mt-5 my-auto">

                <div class="row justify-content-center">
                    <div class="col-6 col-md-10">
                        <img src="icons/nextknowicon.png" class="img-fluid mb-3" alt="nextKnox">
                        <span class="h1 font-weight-bold">
                            nextKnox
                        </span>
                        <p class="h5">Next generation Secure Mobile banking</p>
                    </div>
                </div>
                
            </div>

            <div class="col-12 col-md-6 offset-md-1 mt-5 mt-md-0">
                <img class="img-fluid" src="images/mainImage.png" alt="introimage">
            </div>

            <div class="col-12 col-md-10 offset-md-1">

                <div class="row justify-content-center mt-5">
                    <div class="col-10 col-md-4 mb-4">
                        <button class="btn btn-custom btn-blue pt-3 pb-3 font-weight-bold">Sign up</button>
                    </div>
                    <div class="col-10 col-md-4">
                        <router-link to="/login"><button class="btn btn-custom btn-border-blue pt-3 pb-3 font-weight-bold">Sign in</button></router-link>
                    </div>
                </div>
            </div>

        </div>
    </div>

</template>

<script>


export default {
  name: 'MainBody',
  data(){
      return{
          
      }  
  },   
    components: {
    },
    computed:{

    },  
    methods: {
       
        
    }, 
    mounted(){
        
    }

}
</script>

<style>
    .bg-main{
        background-color: #22272a;
        padding-top: 8rem;
    }
 
    .btn-custom{
        color:white;
        width:100%;
        border-radius: 12px;
        font-size: x-large;
    }
    .btn-blue{
        background-color: #001ec5;
    }
    .btn-border-blue{
        border:solid #001ec5;
    }
     .customInput{
        border-radius: 12px;
        height:56px;
    }
    .customInput:focus,
    .customInput:hover{
        transition:.5s ease;
        
    }
</style>


