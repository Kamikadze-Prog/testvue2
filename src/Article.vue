<template>
<div>
    <article class="ob-tile">
      <div class="ob-wraper"> 
        <h2 id="ob-tile__style">Доставка обедов с eda.ua</h2>
          <div id="ob-tile__text">
            <p>Пришло время обеда, а пойти некуда? Меню всех окрестных заведений приелось, да и времени не так много? 
              А может быть, просто не хочется тратить свое драгоценное время и силы на то, чтобы приготовить обед?
              Закажите обед в офис с бесплатной доставкой!
              Согласно исследованиям РБК около 45% людей заказывают доставку обедов в офис. Это могут быть комплексные обеды, пицца, суши и другие блюда. 
              Конечно, очень важно заботиться о своем здоровье, поэтому лучший выбор - это все-таки заказать комплексные обеды или другую домашнюю еду,
              приготовленная из свежих продуктов по знакомым и любимым рецептам.
            </p>
            <p>Наши партнёры</p>
            <div  class="article__Images">
              <p>Для того, чтобы начать заказывать обеды с доставкой, вы можете самостоятельно выбрать ресторан и сделать первый заказ или позвонить 
                нам по телефону +7 495 783-48-33 и мы с удовольствием вам все расскажем.
                Кроме заказа обедов, мы предоставляем и другие услуги по организации питания.
              </p>
            </div>
          </div>
        </div>
    </article>
</div>
</template>

<script>

export default {
  data () {
      return {
          path: '../assets/Super-Meat-Boy.png',
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  lang="scss">

 .ob-wrapper {
    max-width: 1440px;
    margin: 0 auto;
}

.ob-tile {
    width: 71.3%;
    position: relative;
    margin-top: 0;
    background: #ff7733;
    padding: 33px 20px 55px;
    font-size: 14px;
    margin-left: 10px;
    margin-bottom: 20px;
}

#ob-tile__style {
	padding-top:10px;
     padding-bottom:10px;
    font-size: 20px;
}

#ob-tile__text {
	font-size: 14px;
	line-height: 20px
}

.article__Images img {
    margin-right: 5px;
    height: 50px; 
    width: 50px;
}
</style>
