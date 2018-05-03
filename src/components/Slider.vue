<template>
    <div class="carousel-container text-center">
        <div id="carousel-inner" class="carousel slide" data-ride="carousel" data-interval="4500">
            <!-- bottom ctrls -->
            <ol class="carousel-indicators">
                <li data-target="#carousel-inner" data-slide-to="0" class="active"></li>
                <li data-target="#carousel-inner" data-slide-to="1"></li>
                <li data-target="#carousel-inner" data-slide-to="2"></li>
            </ol>
            <!--  -->
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <!-- ssdsd -->
                    <img class="d-block w-100"  src="./../assets/1.jpg" alt="First slide"/>
                    <h2>Caviar Restaurant</h2>
                    <p>New summer menus available from 12th Sept.</p>
                </div>
                <div class="carousel-item">
                    <img class="d-block w-100" src="./../assets/2.jpg" alt="Second slide"/>
                    <h2>New Menu</h2>
                    <p>Coming up in march!</p>
                </div>
                <div class="carousel-item">
                    <img class="d-block w-100"  src="./../assets/3.jpg" alt="Third slide"/>
                    <h2>Salad Bar</h2>
                    <p>Coming up in march!</p>
                </div>
            </div>
            <!-- left right controls -->
            <a class="carousel-control-prev" href="#carousel-inner" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carousel-inner" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </div>    
</template>

<script>
export default {
  name: 'Slider',
}
</script>

<style lang="sass" scoped>
    .carousel-container
        position: relative
        overflow: hidden
        height: 100vh
    #carousel-inner, .carousel-inner
        height: 100%

    .carousel-item         
        height: 100%
        width: 100%
        img
            height: 100%
            object-fit: cover
        h2  
            z-index: 99
            padding: 10px 30px
            border: 4px solid white
            text-transform: uppercase
            color: white
            left: 50%
            font:
                // weight: bold
            position: absolute
            transform: translate(-50%, -50%)
        p
            position: absolute
            z-index: 99            
            color: white
            left: 50%
            transform: translateX(-50%)
            font:
                family: 'Amita', serif
                style: italic
        &::after
            content: ''
            display: block
            position: absolute
            top: 0
            left: 0
            right: 0
            bottom: 0
            background-color: rgba(0,0,0,0.3)
            
    @media only screen and (min-width: 0)
        .carousel-item         
            h2  
                font-size: 2rem     
                top: 40%
            p
                font-size: 1.5rem     
                top: 55%
    @media only screen and (min-width: 767px)
        .carousel-item         
            h2  
                font-size: 4rem     
            p
                font-size: 2.2rem
                top: 50%
    
    @media only screen and (min-width: 1199px)
        .carousel-item         
            h2  
                font-size: 5rem     
            p
                font-size: 2.2rem
                top: 58%

</style>
