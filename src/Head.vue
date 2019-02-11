<template>
<div>
    <header class="ob-header">
        <div class="ob-wrapper">
            <div class="ob-header__wrap">
                <router-link  :to="{name:'main'}" id="logo-router" class="ob-header__logo"><img  alt="Eda.com" title="Доставка еды" src="./assets/Super-Meat-Boy.png" width="70" id="logo-img">
                </router-link>
                <div class="ob-header__right-content">
                    <div class="ob-header__contacts"><a href="tel:+84044044040" class="ob-header__phone"> {{ contacts }}  <br></a>
                        <span class="ob-header__feedback"> {{ feedback }} </span>
                    </div>
                    <div class="ob-header__login"><a href="#" class="ob-header__btn"> {{login}} </a>
                        <span class="ob-header__login-btn"> {{login_btn}} </span>
                    </div>
                </div>
            </div>
        </div>
    </header>
</div>
</template>

<script>

export default {
  data () {
      return {
          path: '../assets/Super-Meat-Boy.png',
          contacts: '+8 (404) 404-40-40',
          feedback: 'Обратная связь',
          login: 'Компаниям',
          login_btn: 'Войти'
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">
.ob-header {
    background: #fff;
    padding: 0 30px;
    height: 70px;
}

.ob-header__logo {
    display: inline-block;
    padding-top: 0;
    vertical-align: top;
    outline: 0;
}

.ob-header__right-content {
	text-align: right;
    float: right;
    padding-top: 12px;
    height: 55px;
    width: 330px;
}

.ob-header__contacts {
    display: inline-block;
    margin-bottom: 18%;
    padding-right: 18px;
}

.ob-header__phone {
    font-size: 15px;
    text-decoration: none;
    color: #363636;
    display: block;
    font-family: ProximaNova,sans-serif;
}

.ob-header__feedback {
    display: inline-block;
    text-decoration: none;
    border-bottom-width: 1px;
    border-bottom-style: dotted;
    cursor: pointer;
    line-height: .9em;
    color: #999;
    font-size: 12px;
    text-align: right;
}
 .ob-header__feedback:active, .ob-header__feedback:hover {
    color: #000;
    border-bottom-style: none;
}
 
.ob-header__login {
    display: inline-block;
    vertical-align: middle;
}

.ob-header__btn {
    cursor: pointer;
    margin-bottom: 22px;
    padding: 5px 10px;
    margin-right: 4px;
    text-decoration: none;
    font-size: 14px;
    display: inline-block;
    border: 1px solid red;
    color: red;
    line-height: 1.2;
}
 .ob-header__btn:active, .ob-header__btn:hover {
    color: rgb(218, 40, 40);

}

.ob-header__login-btn {
    cursor: pointer;
    padding: 5px 10px;
    text-decoration: none;
    font-size: 14px;
    display: inline-block;
    border: 1px solid red;
    color: red;
}
 
 .ob-header__login-btn:active, .ob-header__login-btn:hover {
    color: rgb(218, 40, 40);
}
 
.ob-nav {
    position: relative;
    background: #ff5f00;
    padding: 3px 0 5px;
    color: #fff;
    white-space: nowrap;
}
.ob-nav__wrap {
    width: 100%;
}

.ob-nav__item {
    display: inline-block;
    width: 60px;
    height: 40px;
    text-align: left;
    border-radius: 2px;

}

.ob-nav__item-active {
    position: relative;
    z-index: 2;
}

.ob-nav__text {
    display: inline-block;
    font-size: 18px;
    padding-top: 6px;
    font-weight: 400px;
    vertical-align: middle;
    font-family: "Open Sans";
    text-overflow: ellipsis;
    overflow: hidden;
    line-height: 12px;
}

.ob-nav__link {
    height: 30px;
    text-decoration: none;
    -webkit-text-decoration-line: none;
    text-decoration-line: none;
    cursor: pointer;
    display: inline-block;
    padding: 4px 10px 5px;
    color: #fff;
}

.ob-nav__list {
    margin-left: 12%;
    vertical-align: middle;
    font-size: 0;
}

.ob-nav__link:active, .ob-nav__link:hover  {
    background: rgb(250, 157, 43);
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

.ob-restaurant-list {
    margin-top: 30px;
}

 .ob-wrapper, {
    max-width: 1440px;
    margin: 0 auto;
}

.ob-restaurant-list__cols {
    font-size: 0;
}
.ob-content {
    padding: 0 10px;
}

.ob-restaurant-list__list {
    width: 74%;
    display: inline-block;
    vertical-align: top;
    margin-right: 2%;
    font-size: 14px;
    margin-bottom: 20px;
}

.b-restaurant-item{
    display: block;
    margin: 0 0 10px 0;
    padding: 20px;
    padding-bottom: 90px;
    background-color: #fff;
    border-radius: 2px;
    text-decoration: none;
    outline: 0;
    transition: box-shadow .8s;
    color: #333;
    font-family: "Open Sans",Arial;
}

.b-restaurant-item__content {
    position: relative;
    display: block;
}

.ob-restaurant-list__sup-col {
    width: 24%;
    display: inline-block;
    vertical-align: top;
    font-size: 14px;
    font-family: "Open Sans";
    font-weight: 400;
    line-height: 20px;
}

.b-restaurant-item__left-column {
    display: flex;
    flex: 0 1 auto;
    -webkit-flex: 0 1 auto;
    -ms-flex: 0 1 auto;
    min-width: 0;
    width: 84%;
}

.b-restaurant-item__overflow {
    margin: 0 20px 0 0;
    overflow: hidden;
    width: 190px;
    height: 120px;
}

.b-restaurant-item__about-column {
    width: 70%;
}

.b-restaurant-item__title  {
    margin: 0 0 5px 0;
    font-size: 20px;
    font-weight: 600;
    line-height: 20px;
    color: #333;
}

.b-restaurant-item__menu {
    position: relative;
    margin: 11px 0 21px 0;
    height: 56px;
}

.b-restaurant-item__menu-list {
    position: absolute;
    width: 100%;
    max-width: 100%;
}

.b-restaurant-item__menu-item  {
    display: block;
}

.b-restaurant-item__item-column {
    font-family: "Open Sans";
    line-height: 21px;
}

.b-restaurant-item__item-name {
    text-overflow: ellipsis;
    white-space: nowrap;
}

.b-restaurant-item__item-text {
    color: #333;
    font-size: 14px;
    font-weight: 400;
}

.b-restaurant-item__item-underline {
    position: relative;
    bottom: 2px;
    margin: 0 2px;
    flex: 1 0 auto;
    -webkit-flex: 1 0 auto;
    -ms-flex: 1 0 auto;
    min-width: 0;
    border-bottom: 1px solid #dedede;
}

.b-restaurant-item__item-price {
    padding-left: 1px;
    color: #333;
    font-size: 14px;
    font-weight: 400;
}

.b-restaurant-item__button {
    position: absolute;
    right: 10px;
    bottom: 35px;
    display: inline-block;
    background-color: #a0c84b;
    padding: 8px 19px;
    color: #fff;
    font-family: "Open Sans",Arial;
    font-size: 14px;
    font-weight: 400;
    line-height: 12px;
}

.ob-restaurant-list__tile {
    background: #fff;
    padding: 20px 20px 20px;
    margin-bottom: 27px;
}
 
.ob-sort-list__title-one {
    margin-bottom: 15px;
    font-weight: 700;
}

.ob-sort-list__label {
    display: block;
    margin-bottom: 15px;
}
 
.ob-tile {
    width: 71.3%;
    position: relative;
	margin-top: 0;
    background: #ff7733;
    padding: 33px 20px 55px;
    font-size: 14px;
    margin-bottom: 20px;
}

#ob-tile__style {
	padding-top:10px;
     padding-bottom:10px;
    font-size: 18px;
}

#ob-tile__text {
	font-size: 14px;
	line-height: 22px
}

.article__Images {
    margin: 0 auto;
    text-align: center;
}

.article__Images img {
    margin-right: 5px;
    height: 50px; 
    width: 50px;
}

footer {
    clear: both;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 60px;
    background-color: #3e3e3e;
    color: #999;
    font-family: 'Open Sans',Arial;
    -webkit-box-shadow: 0px -11px 65px 16px rgba(20,22,26,0.94);
    -moz-box-shadow: 0px -11px 65px 16px rgba(20,22,26,0.94);
    box-shadow: 0px -11px 65px 16px rgba(20,22,26,0.94);
}
.l-contacts {
    border-bottom: 1px solid #5b5b5b;
    margin: 20px 0 28px 0;

}

.b-contacts, .b-copyright, .b-social {
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

.contacts__client {
    width: 339px;
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
