<template>
  <div>

    <div class="gray-back all-screen"></div>
    <div class="row">

      <div class="col-12 border main-dash">

        <div class="row justify-content-center mt-5 pt-5">
          
          <div class="col-5">
            <img src="profilepics/55140896.jpeg" class="img-fluid too-round" alt="">
          </div>

          <div class="col-8 text-center mt-3">
            <span class="h5">Akonofua Osamede</span> <br>
            <span class="h3">0382747583</span> <br>
            <span>Savings</span> <br>
          </div>

          <div class="col-8 act-show pt-4 pb-4 border mb-5 mt-4 text-center font-weight-bold h4">
            $5335352323
          </div>

        </div>

      </div>

      <div class="col-12 mb-5 mt-5 pt-5">
        <div class="row flex-row flex-nowrap pb-4 pt-4 mb-5" style="overflow-x: auto;">

          <div v-for="n in parseInt(numberr)" :key="n" class="col-8 col-md-4 mr-3 ml-3 p-4 border" style="border-radius:50px;">

              <div class="row mb-2">
                <div class="col-12">
                    
                  <div class="row">

                    <span class="h5 col-12 mb-4">Debit</span>

                    <span class="col-12">Date:20/20/12</span>
                    <span class="h3 col-12">To:You</span>
                    <span class="h4 col-12 mb-5">From:you</span>

                    <div class="col-10 offset-1 act-show pt-3 pb-3 mb-3 border text-center">
                      $53353
                    </div>

                  </div>

                </div>     
              </div>

          </div>

        </div>
      </div>

      <!-- lapnavig -->
      <div id="menuFloat" class="gray-back d-none d-md-block">

        <div class="col-12 text-left mt-5">

            <div class="row mt-5">
                <div class="col-12 pl-md-0">
                    <button  class="btn listButtons pt-2 pb-2">
                        <span class="d-flex pl-2"> 
                             <i class="material-icons" style="font-size: 40px;" :class="[inHome ? 'item-selected':'']">home</i>
                            <!--<p class="pt-2  pl-2 nav-text">DashBoard</p>-->
                        </span>
                    </button>
                </div>
            </div>

            <div class="row mt-5">
                <div class="col-12 pl-md-0">
                    <button class="btn listButtons pt-2 pb-2">
                        <span class="d-flex pl-2"> 
                            <i class="material-icons" style="font-size: 40px;" :class="[inTransfer ? 'item-selected':'']">import_export</i>
                            <!--<p class="pt-2  pl-2 nav-text">Requests</p>-->
                        </span>
                    </button>
                </div>
            </div>

            <div class="row mt-5">
                <div class="col-12 pl-md-0">
                    <button  class="btn listButtons pt-2 pb-2">
                        <span class="d-flex pl-2"> 
                            <i class="material-icons" style="font-size: 40px;" :class="[inSetting ? 'item-selected':'']">hexagon</i>
                            <!--<p class="pt-2  pl-2 nav-text">Products</p>-->
                        </span>
                    </button>
                </div>
            </div>

        </div>
        
      </div>

      <div class="unslideothers others d-none d-md-block">

        <div class="col-12">
          <div class="row">

            <div class="col-5 border main-dash">

              <div class="row justify-content-center mt-5 pt-5">
                
                <div class="col-5">
                  <img src="profilepics/55140896.jpeg" class="img-fluid too-round" alt="">
                </div>

                <div class="col-8 text-center mt-3">
                  <span class="h5">Akonofua Osamede</span> <br>
                  <span class="h3">0382747583</span> <br>
                  <span>Savings</span> <br>
                </div>

                <div class="col-8 act-show pt-4 pb-4 border mb-5 mt-4 text-center font-weight-bold h4">
                  $5335352323
                </div>

              </div>

            </div>

            <div class="col-12 mt-5">
              <div class="row flex-row flex-nowrap pb-4 pt-4 mb-5" style="overflow-x: auto;">

                <div v-for="n in parseInt(numberr)" :key="n" class="col-8 col-md-4 mr-3 ml-3 p-4 border" style="border-radius:50px;">

                    <div class="row mb-2">
                      <div class="col-12">
                          
                        <div class="row">

                          <span class="h5 col-12 mb-4">Debit</span>

                          <span class="col-12">Date:20/20/12</span>
                          <span class="h3 col-12">To:You</span>
                          <span class="h4 col-12 mb-5">From:you</span>

                          <div class="col-10 offset-1 act-show pt-3 pb-3 mb-3 border text-center">
                            $53353
                          </div>

                        </div>

                      </div>     
                    </div>

                </div>

              </div>
            </div>

          </div>
        </div>

      </div>

      <!-- bottom navigation -->
      <transition enter-active-class="animate__animated animate__fadeInUp" leave-active-class="animate__animated animate__fadeOutDown">
        <nav class="mobile-bottom-nav d-md-none">

          <div class="mobile-bottom-nav__item">
            <div class="mobile-bottom-nav__item-content">
              <i class="material-icons" style="font-size: 40px;" :class="[inHome ? 'item-selected':'']">home</i>
              <br> 
            </div>		
          </div>

          <div class="mobile-bottom-nav__item">
            <div class="mobile-bottom-nav__item-content">
              <i class="material-icons" style="font-size: 40px;">import_export</i>
              <br>
            </div>		
          </div>

          <div class="mobile-bottom-nav__item">
            <div class="mobile-bottom-nav__item-content">
              <i class="material-icons" style="font-size: 40px;">hexagon</i>
              <br> 
            </div>		
          </div>

        </nav>
      </transition>

    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data(){
    return{
      numberr:10,
      inHome: true, 
      inTransfer:false,
      inSetting:false,
    }
  }
}
</script>

<style scoped>

  .mobile-bottom-nav {
    transition: .5s ease-in;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    will-change: transform;
    transform: translateZ(0);
    display: flex;
    height: 50px;
    background-color: white;
    z-index: 1;
    padding-top:5%;
  }
  .mobile-bottom-nav__item {
    flex-grow: 1;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .mobile-bottom-nav__item--active {
    color: white;
  }
  .mobile-bottom-nav__item-content {
    display: flex;
    flex-direction: column;
  }
  .too-round{
    border-radius: 50%;
  }
  .act-show{
    border-radius:50px;
    background-color: white;
    color:black;
  }
  .main-dash{
    background-color: #0f0f5c;
    color:white;
    border-bottom-left-radius: 100px;
    border-bottom-right-radius: 100px;
  }
  #menuFloat{
    background-color: white;
    position: fixed;
    left:0%;
    width: 100%;
    height: 100%;
    padding-bottom: 10%;
    z-index: 9999 !important;
    top:0%;
    box-shadow:  0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
    .gray-back{
        background-color: #f4f4f4 !important;
        box-shadow: none !important;
    }
 
    .item-selected{
      color:rgb(156, 39, 176);
    }
    .unslideothers{
        width: 100%;
        transform: translateX(0%);
        transition: all .1s linear;
    }
     .others{
        position:fixed;
        height:100%;
        top:10%;
        width:90% !important;
        left:5%;
        overflow-y:scroll;
        background-color: white;
        border-radius: 25px;
        border-bottom-right-radius: 0px;
        z-index: 50000;
        box-shadow: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075) !important;
        }
    @media screen and (min-width:768px){

        .others{
            width:75% !important;
            right:2%;
            left:unset;
            top:5%;
        }
      
    }

</style>