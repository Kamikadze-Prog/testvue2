<template>
<div>
    <header class="ob-header">
        <div class="ob-wrapper">
            <div class="ob-header__wrap">
                <router-link  :to="{name:'#'}" id="logo-router" class="ob-header__logo"><img  alt="Eda.com" title="Доставка еды" src="./assets/Super-Meat-Boy.png" width="70" id="logo-img">
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
    font-family: 'Open Sans',Arial;
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

</style>
