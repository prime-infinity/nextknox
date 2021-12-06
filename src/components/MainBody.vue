<template>

    <div>
        <div class="row bg-main">
            
            <div class="col-md-6 text-white d-none d-md-block bg-main-text">
                <span class="h1">
                    Meet
                </span> <br>
                <span class="h1 font-weight-bold">
                    KnextKnox
                </span> 
            </div>

            <div class="col-12 text-white d-block d-md-none text-center mt-5">
                <span class="h1">
                    Meet
                </span> <br>
                <span class="h1 font-weight-bold">
                    KnextKnox
                </span>
            </div>

            <div class="col-12 col-md-6 offset-md-3">
                <img class="img-fluid" src="/images/mainImage.png" alt="introimage">
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
        height: 100vh;
    }
    .bg-main-text{
        position: absolute;
        top: 20vw;
        left: 10%;
    }
</style>


