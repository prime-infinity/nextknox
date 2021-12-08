<template>
  <div>
    <div class="row">

    <div class="col-11 border">
      <div class="row">

        <div class="col-12">
          <img src="profilepics/55140896.jpeg" class="img-fluid" alt="">
        </div>

      </div>
    </div>

    <!-- bottom navigation -->
    <transition enter-active-class="animate__animated animate__fadeInUp" leave-active-class="animate__animated animate__fadeOutDown">
      <nav class="mobile-bottom-nav">

        <div class="mobile-bottom-nav__item">
          <div class="mobile-bottom-nav__item-content">
            <i class="material-icons" style="font-size: 40px;">home</i>
            <br> 
          </div>		
        </div>

        <div class="mobile-bottom-nav__item">
          <div class="mobile-bottom-nav__item-content">
            <i class="material-icons" style="font-size: 40px;">import_export</i>
            <br> <br><br>
          </div>		
        </div>

        <div class="mobile-bottom-nav__item">
          <div class="mobile-bottom-nav__item-content">
            <i class="material-icons" style="font-size: 40px;">hexagon</i>
            <br> 
          </div>		
        </div>

        <!--<div class="mobile-bottom-nav__item">		
          <div class="mobile-bottom-nav__item-content">
            <i class="las la-user mt-5 mb-4" style="font-size: 40px;"></i>
            <br> 
          </div>
        </div>-->

      </nav>
    </transition>

    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',

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
    background-color: rgb(255, 255, 255);
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

</style>