<template>
<div>
    <section class="ob-content ob-restaurant-list">
        <div class="ob-wrapper">
            <div class="ob-restaurant-list__cols">
                <ul class="ob-restaurant-list__list">
                    <div class="list-view">
                        <div class="items">
                            <div class="b-restaurant-item">
                                <a href="#" class="b-restaurant-item__content">
                                    <div class="b-restaurant-item__left-column">
                                        <div class="b-restaurant-item__image-column">
                                            <div class="b-restaurant-item__image_position">
                                                <div class="b-restaurant-item__overflow">
                                                    <img title="Кафе Vav" class="ob-restaurant-card__logo"  border="0" width="190" src="https://www.rd.com/wp-content/uploads/2018/03/13-Foods-Worth-Trying-at-a-Greek-Restaurant-760x506.jpg" alt="Кафе1">
                                                </div>
                                            </div>
                                        </div>
                                        <div class="b-restaurant-item__about-column">
                                            <div class="b-restaurant-item__title">
                                                <div class="b-restaurant-item__menu">
                                                    <ul class="b-restaurant-item__menu-list">
                                                        <li class="b-restaurant-item__menu-item">
                                                            <ul class="b-restaurant-item__item-column">
                                                                <li class="b-restaurant-item__item-name">
                                                                    <span class="b-restaurant-item__item-text"> Ланч понедельник №1</span></li>
                                                                <li class="b-restaurant-item__item-underline"></li>
                                                                <li class="b-restaurant-item__item-price">287</li>
                                                            </ul>
                                                        </li>
                                                        <li class="b-restaurant-item__menu-item">
                                                            <ul class="b-restaurant-item__item-column">
                                                                <li class="b-restaurant-item__item-name">
                                                                    <span class="b-restaurant-item__item-text">Борщ с говядиной (ежедневно)</span></li>
                                                                <li class="b-restaurant-item__item-underline"></li>
                                                                <li class="b-restaurant-item__item-price">109</li>
                                                            </ul>
                                                        </li>
                                                        <li class="b-restaurant-item__menu-item">
                                                            <ul class="b-restaurant-item__item-column">
                                                                <li class="b-restaurant-item__item-name">
                                                                    <span class="b-restaurant-item__item-text">Ланч четверг №2 </span></li>
                                                                <li class="b-restaurant-item__item-underline"></li>
                                                                <li class="b-restaurant-item__item-price">289</li>
                                                            </ul>
                                                        </li>
                                                    </ul>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="b-restaurant-item__button">Меню</div>
                                </a>
                            </div>
                        </div>
                    </div>
                </ul>
                <div class="ob-restaurant-list__sup-col">
                    <div class="ob-restaurant-list__tile ob-restaurant-list__tile-sort">
                        <span class="ob-restaurant-list__timer-icon"></span>
                        <div class="ob-sort-list__wrapper">
                            <div class="ob-sort-list__title-one">Сортировка</div>
                            <div class="js-sort-list-checkbox">
                                <label class="ob-sort-list__label">
                                    <input type="radio" class="ob-radio__field" name="sort-item" data-sort="rating" value="rating" checked="">
                                    <span class="ob-radio__text">по рейтингу</span>
                                </label>
                                <label class="ob-sort-list__label">
                                    <input type="radio" class="ob-radio__field" data-sort="min_sum" name="sort-item" value="min_sum">
                                    <span class="ob-radio__text">по минимальной сумме</span>
                                </label>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
         </div>
         </section>   
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

.ob-restaurant-list {
    margin-top: 30px;
}

 .ob-wrapper {
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
    width: 81.5%;
    display: inline-block;
    vertical-align: top;
    margin-right: 1%;
    font-size: 14px;
    margin-top: 0;
    margin-bottom: 20px;
    padding-left: 0; 
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
    font-family: 'Open Sans',Arial;
}

.b-restaurant-item__content {
    position: relative;
    display: block;
}

.ob-restaurant-list__sup-col {
    width: 17.5%;
    display: inline-block;
    vertical-align: top;
    font-size: 14px;
    font-family: 'Open Sans',Arial;
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
    font-family: 'Open Sans',Arial;
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
    min-width: 0;
    font-family: 'Open Sans',Arial;
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
</style>
