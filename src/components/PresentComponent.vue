<script></script>

<template>
  <section class="present">
    <h2 class="present__heading">PDF-презентация дома</h2>
    <p class="present__text">Скачайте презентацию, в которой мы собрали всю информацию<br>
      по объекту: расположение, планировка, преимущества и цены</p>
    <a class="present__download" href="#!">Скачать презентацию</a>
    <div class="present__slider">
      <article class="present__slide">
        <img src="/images/slide-1.jpg" width="320" height="321" alt="Слайд дома (ванная).">
        <div class="slide__content content">
          <h3 class="content__heading">Экологичный дом<br> по дизайн-проекту</h3>
          <p class="content__text">Строительство и отделка дома осуществлялись по дизайн-проекту с сопровождением.
            Система канализации своя, автономная.
            По проекту построены локальные очистные сооружения, техническая вода выходит в чистом виде на полив
            растительности и обратно возвращается в бачок унитаза, что позволяет экономить воду.</p>
          <div class="slider__control">
            <button class="prev">
              <span class="visually-hidden">Предыдущий слайд.</span>
            </button>
            <span class="counter">1 / 12</span>
            <button class="next">
              <span class="visually-hidden">Следующий слайд.</span>
            </button>
          </div>
        </div>
      </article>
    </div>
  </section>
</template>

<style lang="scss">
.present {
  padding-bottom: 27px;
  background-color: #e2e2e2;
  background-image: url("../images/present-bg-mobile.jpg");
  background-repeat: no-repeat;
}

.present__heading {
  margin-bottom: 20px;
  font-size: 24px;
  line-height: 120%;
  font-weight: 900;
  text-align: center;
}

.present__text {
  margin: 0 30px;
  margin-bottom: 40px;
  font-size: 16px;
  line-height: 120%;
  color: #35465e;
}

.present__download {
  margin: 0 30px;
  display: block;
  width: 251px;
  height: 49px;
  padding: 15px 20px;
  padding-left: 50px;
  box-sizing: border-box;
  background-color: #2489ff;
  border-radius: 5px;
  font-family: "Roboto", "Arial", sans-serif;
  font-size: 16px;
  line-height: 120%;
  color: #ebebeb;
  text-align: center;
  position: relative;

  &::before {
    position: absolute;
    content: "";
    top: 16px;
    left: 34px;
    width: 15px;
    height: 15px;
    background-image: url("../images/download-icon-mobile.svg");
  }
}

.present__slider {
  padding-top: 400px;
}

.slide__content {
  width: 300px;
  position: relative;
  top: -40px;
  margin: 0 auto;
  padding: 30px;
  box-sizing: border-box;
  background-color: #ffffff;
  border-radius: 5px;
}

.content__heading {
  margin-bottom: 15px;
  font-weight: 900;
  font-size: 18px;
  line-height: 120%;
}

.content__text {
  margin-bottom: 30px;
  font-size: 14px;
  line-height: 120%;
  font-weight: 200;
  color: #35465e;
}

.prev,
.next {
  border: none;
  background: none;
  width: 20px;
  height: 14px;
  background-image: url("../images/slider-page-arrow-left.svg");
  cursor: pointer;
}

.next {
  transform: scale(-1);
}

.counter {
  font-size: 15px;
  line-height: 120%;
  padding: 0 20px;
}
</style>