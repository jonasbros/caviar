<template>
  <div class="container-fluid">
      <slider/>

      <section class="s1 row text-center">
        <div class="col-lg-6">
            <h2 class="mb-5">GASTRO BAR</h2>
            <h5 class="mb-4">
                The exciting tastes of international cuisine in a superb interior of our newly opened Brooklyn gastro bar. The newly gentrified neighbourhood offers beautiful views.
            </h5>
            <p class="mb-5">
                Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round. Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.
            </p>
            <button type="button" class="btn btn-outline-dark mb-5">Find out more</button>
        </div>
        <div class="img-part col-lg-6 clearfix">
            <img class="col-lg-6 mb-3" src="./../assets/s1-1.jpg">
            <img class="col-lg-6 mb-5" src="./../assets/s1-2.jpg">
        </div>       
      </section>

      <section class="s2 row text-left">
          <div class="img-part col-lg-6 px-5">
              <img src="../assets/s2-2.jpeg">
          </div>
          <div class="col-lg-6 px-5">
              <h2 class="text-white my-lg-5 mt-3 mb-5">AWARD WINNING CHEFS</h2>
              <h5 class="mb-4">
                  The exciting tastes of international cuisine in a superb interior of our newly opened Brooklyn gastro bar. The newly gentrified
              </h5>
              <p class="mb-5">
                  Gochujang cliche skateboard cred. Kombucha food truck raw denim listicle, authentic bicycle rights la croix chia. Tattooed single-origin coffee poutine bespoke trust fund typewriter.
              </p>
              <button type="button" class="btn mb-5">See menus</button>
          </div>
      </section>

      <section class="s3 row text-center">
          <div class="mb-5 col-12">
              <h2 class="mb-5">Reviews</h2>
              <h5 class="mb-5">The exciting tastes of international cuisine in a superb interior of our newly opened Brooklyn gastro bar.</h5>
                <div id="s3-carousel" class="carousel slide col-12" data-ride="carousel">
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <div style="background-image: url('https://randomuser.me/api/portraits/men/82.jpg')"></div>
                            <p class="text-muted mb-4">We are made wise not by the recollection of our past, but by the responsibility for our future.</p>
                            <p><strong>RALPH HARRIS</strong></p>
                        </div>            
                        <div class="carousel-item ">
                            <div style="background-image: url('https://randomuser.me/api/portraits/women/57.jpg')"></div>
                            <p class="text-muted mb-4">We are made wise not by the recollection of our past, but by the responsibility for our future.</p>
                            <p><strong>JANICE JOHNSON</strong></p>
                        </div>                    
                        <div class="carousel-item ">
                            <div style="background-image: url('https://randomuser.me/api/portraits/men/86.jpg')"></div>
                            <p class="text-muted mb-4">We are made wise not by the recollection of our past, but by the responsibility for our future.</p>
                            <p><strong>JOHN ALBERTSON</strong></p>
                        </div>
                    </div>
                    <a class="carousel-control-prev" href="#s3-carousel" role="button" data-slide="prev">
                        <i class="fas fa-angle-left"></i>
                        <span class="sr-only">Previous</span>
                    </a>
                    <a class="carousel-control-next" href="#s3-carousel" role="button" data-slide="next">
                        <i class="fas fa-angle-right"></i>
                        <span class="sr-only">Next</span>
                    </a>
                </div>
          </div>
      </section>

      <section class="s4 row text-left">
          <div class="col-lg-3">
              <p>EASY BREAKFAST</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
          <div class="col-lg-3">
              <p>HEALTY FOOD</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
          <div class="col-lg-3">
              <p>MAIN DISH</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
          <div class="col-lg-3">
              <p>GREEN JUICE LEGGINGS</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>

          <div class="col-lg-3">
              <p>EASY BREAKFAST</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
          <div class="col-lg-3">
              <p>EASY BREAKFAST</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
          <div class="col-lg-3">
              <p>EASY BREAKFAST</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
          <div class="col-lg-3">
              <p>EASY BREAKFAST</p>
              <p>Sometimes the simplest things are the hardest to find. So we created a new line for everyday life, All Year Round.</p>
          </div>
      </section>

        <section class="s5 row text-center">
            <div class="col-12">
                <h2 class="mb-5">Follow Us</h2>
                <i class="fab fa-facebook-f"></i>
                <i class="fab fa-twitter"></i>
                <i class="fab fa-pinterest-p"></i>
                <i class="fab fa-google-plus-g"></i>
                <i class="fab fa-instagram"></i>
            </div>      
        </section>

        <section class="s6 row">
            <div class="col-12 text-center">
                <li>
                <span><small><i class="fas fa-phone"></i>RESERVATIONS: 011 678 67856</small></span>
                </li>
                <li>
                    <span><small><i class="far fa-clock"></i>MON - SAT 8.00 - SUNDAY CLOSED</small></span>
                </li>
            </div>
        </section>
  </div>
</template>

<script>
import slider from './Slider';
export default {
    name: 'Home',
    components: {
        slider,
    }
}
</script>

<style lang="sass" scoped>
    *
        overflow: hidden
    .container-fluid
        padding: 0
    section
        .img-part img
            display: block
            object-fit: cover  
            position: relative
            z-index: 99      
        div
            overflow: hidden
            h5
                font:
                    family: 'Amita', sans-serif
                    style: italic
            h2
                &::after
                    content: ""
                    width: 8%
                    height: 3px
                    background-color: #2d2d2d
                    display: block
                    position: absolute
                    left: 50%
                    z-index: 999
                    transform: translate(-50%, 200%)
    .s2
        position: relative
        background:
            image: url(../assets/s2-1.jpeg)
            size: cover
            position: center center
            attachment: fixed
        color: #f2f2f2
        &::before
            content: ''
            display: block
            position: absolute
            top: 0
            left: 0
            right: 0
            bottom: 0
            background-color: rgba(0,0,0,0.325)
        h2
            &::after
                background-color: #f2f2f2
    .s3
        h5
            margin: 0 auto
        #s3-carousel
            height: 100%
            i
                color: #2d2d2d
                font-size: 3rem
            .carousel-item
                div
                    margin: 20px auto
                    height: 128px
                    width: 128px
                    border-radius: 69%
                    background:
                        size: cover
                        position: center center
                p
                    margin: 0 auto
                
    .s4
        color: white
        position: relative
        background:
            image: url('../assets/s4-1.jpg')
            size: cover
            position: center center
            attachment: fixed
        &::before
            content: ''
            display: block
            position: absolute
            top: 0
            left: 0
            right: 0
            bottom: 0
            background-color: rgba(0,0,0,0.325)
        div 
            margin-bottom: 20px
    .s5 
        // padding: 40px
        background-color: rgba(23, 27, 44, 1)
        color: white
        i
            font-size: 1.3rem
            margin: 0 20px
        h2::after
            background-color: #f2f2f2
    
    .s6
        background-color: rgba(23, 27, 44, 1)
        color: #f2f2f2
        div
            float: left
            display: inline-block
        li, i
            vertical-align: middle
            list-style: none
            display: inline-block
            margin-right: 5px

    @media only screen and (min-width: 0)
        section
            padding: 40px 15px
            .img-part
                height: auto
                img
                    float: none
                    height: 50%
                    width: 100%
        .s2 
            .img-part img    
                height: 100%
            h2
                &::after
                    left: 20%
            div
                height: auto
        .s5
            padding: 20px 0
        .s6
            padding: 0 20px
            height: 60px


    @media only screen and (min-width: 992px)
        section
            padding: 80px 180px
            .img-part img
                float: left
                height: 100%               
        .s2
            height: 80vh
            h2
                &::after
                    left: 12%
        .s3
            height: 90vh
            h5
                width: 50%
            // padding: 80px
            .carousel-item p
                width: 30%
        .s4
            height: 65vh
        .s5
            padding: 40px
            height: 30vh
        .s6
            height: 60px
            padding: 10px 15px
</style>
