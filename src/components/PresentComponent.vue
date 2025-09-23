<script></script>

<template>
  <section class="present">
    <div class="present__wrap">
      <h2 class="present__heading">PDF-презентация дома</h2>
      <p class="present__text">Скачайте презентацию, в которой мы собрали всю информацию<br class="br-mobile">
        по объекту: расположение, планировка, преимущества и цены</p>
      <a class="present__download" href="#!">Скачать презентацию</a>
    </div>
    <div class="present__slider">
      <article class="present__slide">
        <picture>
          <source srcset="/images/slide-desktop-1.jpg" width="1440" height="877" media="(min-width: 1440px)">
          <img src="/images/slide-1.jpg" width="320" height="321" alt="Слайд дома (ванная).">
        </picture>
        <div class="slide__content content">
          <h3 class="content__heading">Экологичный дом<br class="br-mobile"> по дизайн-проекту</h3>
          <p class="content__text">Строительство и отделка дома осуществлялись по <br class="br-desktop"> дизайн-проекту
            с сопровождением.
            Система<br class="br-desktop"> канализации своя, автономная.<br class="br-desktop">
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

  @media (min-width: 1440px) {
    padding-top: 32px;
    background: none;
  }
}

.present__wrap {
  display: contents;

  @media (min-width: 1440px) {
    display: block;
    width: 950px;
    height: 367px;
    margin: 0 auto;
    padding-top: 70px;
    padding-left: 66px;
    box-sizing: border-box;
    background-image: url("../images/present-bg-desktop.jpg");
    background-repeat: no-repeat;
    background-position: 100% 100%;
    box-shadow: 0 10px 5px 10px rgba(#000000, 0.2);
  }
}

.present__heading {
  margin-bottom: 20px;
  font-size: 24px;
  line-height: 120%;
  font-weight: 900;
  text-align: center;

  @media (min-width: 1440px) {
    margin-bottom: 13px;
    font-size: 36px;
    text-align: left;
    color: #35465e;
  }
}

.present__text {
  margin: 0 30px;
  margin-bottom: 40px;
  font-size: 16px;
  line-height: 120%;
  color: #35465e;

  @media (min-width: 1440px) {
    margin: 0;
    width: 400px;
    margin-bottom: 32px;
    font-size: 18px;
    line-height: 140%;
  }
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

  @media (min-width: 1440px) {
    width: 318px;
    height: 66px;
    margin: 0;
    padding: 24px 20px;

    &::before {
      top: 25px;
      left: 40px;
    }
  }
}

.present__slider {
  padding-top: 400px;

  @media (min-width: 1440px) {
    padding-top: 168px;
  }
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

  @media (min-width: 1440px) {
    top: -214px;
    margin-left: 147px;
    width: 558px;
    height: 414px;
    padding: 50px;
    box-sizing: border-box;
    box-shadow: 0 8px 14px rgba(#35465e, 0.02),
      0 50px 80px rgba(#35465e, 0.1);
  }
}

.content__heading {
  margin-bottom: 15px;
  font-weight: 900;
  font-size: 18px;
  line-height: 120%;

  @media (min-width: 1440px) {
    font-size: 24px;
    color: #35465e;
    margin-bottom: 29px;
  }
}

.content__text {
  margin-bottom: 30px;
  font-size: 14px;
  line-height: 120%;
  font-weight: 200;
  color: #35465e;

  @media (min-width: 1440px) {
    font-size: 16px;
    line-height: 172%;
    margin-bottom: 41px;
  }
}

.prev,
.next {
  border: none;
  background: none;
  width: 20px;
  height: 14px;
  background-image: url("../images/slider-page-arrow-left.svg");
  cursor: pointer;

  @media (min-width: 1440px) {
    width: 40px;
    height: 24px;
    background-image: url("../images/arrow-prev-desktop.svg");
  }
}

.next {
  transform: scale(-1);
}

.counter {
  font-size: 15px;
  line-height: 120%;
  padding: 0 20px;

  @media (min-width: 1440px) {
    font-size: 21px;
  }
}
</style>