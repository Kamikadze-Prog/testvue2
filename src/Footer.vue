<template>
<div>
    <footer class="footer_style">
        <div class="l-contacts">
            <div class="b-contacts"> 
                <ul class="contacts clearfix"> 
                    <li class="contacts__item contacts__client"> 
                        <a href="tel:+4 404 404-40-40" class="contacts__phone-number">+4 404 404-40-40</a> 
                        <span class="contacts__text">(клиентам)</span> 
                    </li> 
                    <li class="contacts__item contacts__partners"> 
                        <a href="tel:+4 404 404-40-40" class="contacts__phone-number">+5 505 505-50-50</a> 
                        <span class="contacts__text">(партнерам)</span> 
                    </li> 
                    <li class="contacts__item contacts-feedback"> 
                        <div class="contacts__feedback">Обратная связь</div> 
                    </li> 
                </ul> 
            </div> 
        </div> 
    </footer>
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
.footer_style {
    clear: both;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 60px;
    background-color: #3e3e3e;
    color: #999;
    font-family: 'Open Sans',Arial;
    box-shadow: 0px -20px 87px -14px rgba(0, 22, 26, 0.94);

}
.l-contacts {
    margin: 20px 0 38px 0;
    padding-top: 1px;

}

.b-contacts {
    margin: 0 auto;
    width: 1200px;
}

.contacts {
    margin: 0 0 20px 0;
    padding: 0;
    color: red;
}
 
 
.contacts__item {
    float: left;
    margin: 0;
    padding: 0;
    width: 294px;
    list-style-type: none;
}

.contacts__phone-number {
    display: inline-block;
    text-decoration: none;
    color: #fff;
    line-height: 37px;
    font-size: 24px;
}

.contacts__client {
    width: 340px;
}
.contacts__partners {
    width: 340px;
}

.contacts__text {
    color: #dedede;
    font-size: 18px;
    font-weight: 400;
    display: inline-block;
    margin: -1px 0 0 4px;
}
 
 .contacts__feedback {
    width: 350px;
    height: 38px;
    padding: 11px 0 0 0;
    color: #dedede;
    font-size: 18px;
    font-weight: 400;
    line-height: 20px;
    box-sizing: border-box;
    border: 1px solid #5b5b5b;
    border-radius: 3px;
    text-align: center;
    cursor: pointer;
}
</style>
