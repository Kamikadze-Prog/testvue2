<template>
<div>
    <div class="banner-container">
        <div class="banner-inner-wrapper">
            <div class="banner-breadcrumbs">
                <div class="ob-breadcrumbs">
                </div>
            </div>
            <div class="banner-inline">
                <h1> <span id="banner-Text1">все рестораны</span> <br><span id="banner-Text2">заказ и доставка в вашем городе</span></h1>
            </div>
        </div>
    </div>
</div>    
</template>

<script>

export default {
  data () {
      return {

      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">

.banner-container {
    background-position: 0 10%;
    background-repeat: no-repeat;
    background-size: cover;
    height: 250px;
    width: 100%;
    position: relative;
    margin: 0 0 10px 0;
}

.banner-container {
    background-image: url(https://png.pngtree.com/thumb_back/fw800/back_pic/02/66/74/52578b688503f53.jpg);
}

.banner-breadcrumbs {
    display: block;
    position: absolute;
    top: 0;
    height: 30px;
    margin-top: 10px;
}

.banner-inner-wrapper {
    padding: 0 110px;
    margin: 0 auto;
    max-width: 1440px;
}

.banner-inner-wrapper:before {
    content: '';
    height: 250px;
    display: inline-block;
    vertical-align: middle;
}

.banner-inline {
    display: inline-block;
    width: 90%;
    vertical-align: middle;
}

h1 {
    display: block;
    font-size: 28px;
    margin-block-start: 1em;
    margin-block-end: 1em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    color: #fff;
    font-weight: bold;
}

#banner-Text1 {
    display: inline-block;
    font-size: 36px;
    font-weight: 700;
    color: #000000;
    text-shadow: white 0 0 2px;
    line-height: 45px;
    text-transform: uppercase;
    width: 55%;
}

#banner-Text2 {
    display: inline-block;
    font-size: 28px;
    color: #000000;
    text-shadow: white 0 0 2px;
    line-height: 45px;
}
</style>
