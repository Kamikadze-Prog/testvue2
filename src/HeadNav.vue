<template>
<div>
    <nav class="ob-nav ">
        <div class="ob-wraper">
            <div class="ob-nav__wrap"> 
                <ul class="ob-nav__list ">
                    <li class="ob-nav__item">
                            <a href="#" class="ob-nav__link" data-route="all" title="<Бизнеc ланч">
                            <span class="ob-nav__text">{{nav_lunch}}</span>
                        </a>
                    </li>
                    <li class="ob-nav__item ob-nav__item-active">
                        <a href="#" class="ob-nav__link" data-route="20" title="Ресторан">
                            <span class="ob-nav__text"> {{nav_restaurant}}</span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</div>
</template>

<script>

export default {
  data () {
      return {
          nav_lunch: 'Ланч',
          nav_restaurant: 'Ресторан'
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">

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
</style>
