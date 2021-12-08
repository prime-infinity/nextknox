<template>

    <div>
        <div class="row bg-main pb-5">
            
            <div class="col-12 col-md-5 text-center my-auto">

                <div class="row">

                    <div class="col-10 offset-1 offset-md-2">

                        <div class="row justify-content-center d-md-none">
                            <div class="col-5">
                                <img src="icons/nextknowiconedited.png" class="img-fluid mb-3" alt="nextKnox">
                            </div>
                        </div>
                        <div class="row d-none d-md-block">
                            <div class="col-6">
                                <img src="icons/nextknowiconedited.png" class="img-fluid mb-3" alt="nextKnox">
                            </div>
                        </div>

                        <div class="text-md-left text-center">
                            <span class="h1 font-weight-bold">
                                nextKnox
                            </span>
                            <p class="h5">Next generation Secure Mobile banking <br>
                            All At your fingertips </p>
                        </div>

                    </div>

                </div>
                
            </div>

            <div class="col-12 col-md-5 offset-md-1 mt-md-0">
                <img class="img-fluid" src="images/mainImage.png" alt="introimage">
            </div>

            <div class="col-12 col-md-10 offset-md-1">

                <div class="row justify-content-center mt-5 pt-5 mb-5">
                    <div class="col-10 col-md-6">
                        <router-link to="/login"><button class="btn btn-custom pt-3 pb-3 font-weight-bold">Get Started</button></router-link>
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
        /*background-color: #22272a;*/
        padding-top: 8rem;
        background-color:white;
    }
 
    .btn-custom{
        width:100%;
        border-radius: 100px;
        font-size:large;
        background-color: #0023c4;
        color:white;
    }

</style>


