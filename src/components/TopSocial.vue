<template>
  <div class="container-fluid mt-lg-0 mt-sm-5 d-none d-sm-block">
        <div class="i-container">
            <li>
                <span><small><i class="fas fa-phone"></i>RESERVATIONS: 011 678 67856</small></span>
            </li>
            <li>
                <span><small><i class="far fa-clock"></i>MON - SAT 8.00 - SUNDAY CLOSED</small></span>
            </li>
        </div>
        <div class="i-container text-right">
            <span style="margin-right: 10px;"><small>CONNECT WITH US</small></span>
            <li><span><small><i class="fab fa-facebook-f"></i></small></span></li>
            <li><span><small><i class="fab fa-twitter"></i></small></span></li>
            <li><span><small><i class="fab fa-pinterest-p"></i></small></span></li>
            <li><span><small><i class="fab fa-google-plus-g"></i></small></span></li>
            <li><span><small><i class="fab fa-instagram"></i></small></span></li>
        </div>
  </div>
</template>

<script>
export default {
  

}
</script>

<style lang="sass" scoped>
    .container-fluid
        background-color: transparent
        height: 25px
        position: absolute
        top: 0
        z-index: 99
        color: white
        padding-top: 10px
    li:last-of-type
        margin: 0
    li
        list-style: none
        display: inline-block
        margin-right: 10px
        i
            margin-right: 8px
    .i-container
        width: 50%
        display: inline-block
        float: left

    @media only screen and (max-width: 992px)
        .i-container li, span
            font-size: .9rem

</style>
