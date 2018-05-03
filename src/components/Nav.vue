<template>
<nav class="navbar navbar-expand-lg fixed-top mt-lg-4">
  <div class="navbar-brand-container text-center d-none d-lg-block">
    <a class="navbar-brand" href="#">C</a>
  </div>
  
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto ml-auto">
      <li class="nav-item active">
        <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">About</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">The Chefs</a>
      </li>    
      <li class="nav-item">
        <a class="nav-link" href="#">Blog</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Contact</a>
      </li>
    </ul>
  </div>
</nav>
</template>

<script>
export default {
  name: 'Nav',
  data() {
    return {
      sw: window.screen.width,
    }
  },
  mounted() {
    var brand = document.querySelector('.navbar-brand-container');
    var ntrigger = brand.offsetTop + brand.offsetHeight;
    var slider = document.querySelector('.carousel-container');
    var strigger = slider.offsetTop + slider.offsetHeight;
    //nav scrolling
    window.onscroll = function() {     
      if( window.scrollY >= ntrigger + 80 && this.sw > 992 ) {
        $(brand).css('transform', 'scale(0)');      
        $(brand).css('color', 'white');
        
        setTimeout( function() {          
          if( !$(brand).find('.navbar-brand').hasClass('d-none') ) {
            $(brand).find('.navbar-brand').addClass('d-none');  
            $(brand).parent().removeClass('mt-lg-4').addClass('mt-lg-0');
          }
        }, 250);
      }
      
      if( window.scrollY <= ntrigger && this.sw > 992 ) {          
        $(brand).css('transform', 'scale(1)');
        
        setTimeout( function() {       
        if( $(brand).find('.navbar-brand').hasClass('d-none') ) {
          $(brand).parent().removeClass('mt-lg-0').addClass('mt-lg-4');
          $(brand).find('.navbar-brand').removeClass('d-none');
        } 
        }, 250);
      }
      /* change nav colors */
      if( this.sw > 992 && window.scrollY >= strigger ) {
        $(brand).parent().removeClass('navbar-dark').addClass('navbar-light');
        $(brand).parent().addClass('over-slider');
      }else if( this.sw > 992 && window.scrollY <= strigger ) {
        $(brand).parent().removeClass('navbar-light').addClass('navbar-dark');
        $(brand).parent().removeClass('over-slider');
      }
  
    }.bind(this);
    //on resize
    window.onresize = function() {
      this.sw = window.screen.width;

      if( this.sw < 992 ) {
        $(brand).parent().removeClass('navbar-dark').addClass('bg-light navbar-light');
      }else {
        $(brand).parent().addClass('navbar-dark').removeClass('bg-light navbar-light');
      }
    }.bind(this);

    if( this.sw < 992 ) {
      $(brand).parent().addClass('bg-light navbar-light');
    }else {
      $(brand).parent().addClass('navbar-dark');
    }
  },
  methods: {

  }
}
</script>

<style lang="sass" scoped>
  .navbar
    display: block
    background-color: transparent
    text-transform: uppercase
    color: white
    font:
      weight: bold
      size: 1.1rem
  .navbar-brand-container
    display: block
    width: 100%
    margin-bottom: 15px
    transform: scale(1)
    transition: transform 1s
    a
      color: #2d2d2d
      font:
        size: 3rem
        weight: bold
      // border: 5px solid #fff
      background-color: #fff
      padding: 0px 22px
    // clear: both
  .navbar-collapse
    width: 100%
    clear: both    
  .nav-item
    margin-right: 30px 

  .over-slider
    background-color: white
    box-shadow: 0px 0px 1px 0px grey


</style>
