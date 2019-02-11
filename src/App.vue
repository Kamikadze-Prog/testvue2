<template>
  <div id="app">
    <app-head></app-head>
    <app-nav></app-nav>
        <div class="l-search-address">
          <div class="b-search-address" data-is-address="0">
            <div class="search-address search-address_big ">
              <div class="search-address__marker">
                <img src="#" alt="search">
              </div>
              <div class="search-address__title">Лучшие предложения рядом</div>
              <div class="search-address__form clearfix">
                <div class="search-address__wrapper-feild">
                    <div class="search-address__wrap-shake">
                        <input type="text" class="search-address__feild" placeholder="Укажите улицу и дом" data-address-id="" value="" data-geo="">
                    </div>
                    <div class="search-address__wrap-hint-address">
                        <div class="search-address__hint-address">
                            Пожалуйста, укажите улицу и дом
                        </div>
                    </div>
                </div>
                <div class="search-address__button">
                    <div class="search-address__button-text">Я здесь</div>
                </div>
              </div>
          </div>
          <div class="found-address search-address__hide">
              <div class="found-address__text">
                  <span class="found-address__string">
                      <span class="found-address__location"></span><span class="found-address__address"></span>
                  </span>
              </div>
          </div>
        </div>
      </div>
      <app-banner></app-banner>
      <app-content></app-content>
      <app-article></app-article>
      <app-footer></app-footer>
  </div>
</template>

<script>
import Head from './Head.vue'
import HeadNav from './HeadNav.vue'
import Banner from './Banner.vue'
import ContentList from './ContentList.vue'
import Article from './Article.vue'
import Footer from './Footer.vue'

export default {
  data () {
    return {

      }
    },
    components: {
      appHead: Head,
      appNav: HeadNav,
      appBanner: Banner,
      appContent: ContentList,
      appArticle: Article,
      appFooter: Footer
    }
}
</script>

<style lang="scss">

body {
    margin: 0;
    padding: 0;
    border: 0;
    position: relative;
    font-family: Arial,sans-serif;
    font-size: 14px;
    color: #363636;
    line-height: 1.2;
    background: #f1f1f1;
    width: 100%;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
} 

a {
    text-decoration: none;
    cursor: pointer;
    line-height: .9em;
    color: #ff5f00;
    font-size: 12px;
}

.b-search-address .search-address {
    margin: 0 auto;
    max-width: 1440px;
}

.l-search-address {
    background-color: #302829;
    transition: top .3s;
}

.b-search-address {
    padding: 8px 20px 6px 20px;
    z-index: 3;
}

.b-search-address .error-address {
    margin: 12px auto;
    max-width: 1440px;
    color: red;
}

.b-search-address .search-address__hide {
    display: none;
}

.search-address__hide {
    display: none;
}

 .b-search-address .search-address__marker {
    float: left;
    margin: 3px 10px 0 0;
    width: 16px;
    height: 24px;
    background-image: url(/img/location.png);
    background-size: cover;
}

.b-search-address .search-address__title {
    margin: 0 0 9px 0;
    color: #fff;
    font-size: 18px;
    font-weight: 600;
    line-height: 22px;
    box-sizing: border-box;
}

.b-search-address .search-address__form {
    position: relative;
}

.b-search-address .search-address__wrapper-feild {
    position: relative;
    margin: 0 85px 6px 0;
    box-sizing: border-box;
}

.b-search-address .search-address__wrap-shake {
    background-color: #fff;
    margin: 0 -6px 0 0;
}

.b-search-address .search-address__wrap-hint-address {
    display: none;
    position: absolute;
    bottom: -37px;
    padding: 3px 8px;
    color: #fff;
    font-size: 12px;
    font-weight: 400;
    background-color: #ff5f00;
    border-radius: 3px;
    z-index: 1;
}

.b-search-address .search-address__list {
    display: none;
    width: 100%;
    position: absolute;
    left: 1px;
    overflow-y: auto;
    background-color: #fff;
    outline: 1px solid #dedede;
    box-shadow: 0 5px 10px rgba(0,0,0,.1);
    z-index: 25;
}

.b-search-address .found-address {
    margin: 0 auto;
    max-width: 1440px;
}

.b-search-address .found-address__text {
    font-size: 14px;
    font-weight: 400;
    line-height: 22px;
}

.b-search-address .search-address__hint-address {
    position: relative;
    padding: 5px 0 5px 0;
}

.b-search-address .search-address__button {
    position: absolute;
    right: 0;
    bottom: 0;
    width: 79px;
    height: 30px;
    background-color: #a0c84b;
    border: 0;
    cursor: pointer;
}

.b-search-address .search-address__button-text {
    color: #fff;
    text-align: center;
    font-size: 16px;
    font-weight: 400;
    line-height: 29px;
}

.b-search-address .found-address__string {
    position: relative;
    padding: 5px 0;
    color: #fff;
    font-size: 24px;
    border-radius: 3px;
    cursor: pointer;
}

.b-search-address .search-address__feild {
    width: 100%;
    height: 30px;
    padding: 0 6px 0 37px;
    box-sizing: border-box;
    background-color: #fff;
    background: url(http://www.clker.com/cliparts/v/4/S/w/5/p/navigation-md.png) 10px 5px no-repeat;
    background-size: 20px 20px;
    color: #333;
    font-size: 18px;
    font-weight: 400;
    line-height: 22px;
    border: 0;
    outline: 0;
    border-radius: 0;
    -webkit-appearance: none;
}

.b-search-address .found-address__location {
    display: inline-block;
    margin: 0 10px -5px 0;
    width: 16px;
    height: 24px;
    background-image: url(http://pluspng.com/img-png/png-location-location-black-png-image-4231-1200.png);
    background-size: cover;
}

</style>
