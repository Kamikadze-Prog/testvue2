<template>
<div>
    <nav class="ob-nav ">
        <div class="ob-wraper">
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

.ob-wraper {
    margin: 0 auto;
    max-width: 1440px;
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
    padding-left: 0;
    margin-left: 5px;
    vertical-align: middle;
    font-size: 0;
}

.ob-nav__link:active, .ob-nav__link:hover  {
    background: rgb(250, 157, 43);
}
</style>
