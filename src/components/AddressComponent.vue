<script></script>

<template>
  <section class="address">
    <h2 class="visually-hidden">Наше расположение</h2>
    <div class="address__wrap">
      <p class="address__o">Объект находится<br class="br-mobile"> по адресу</p>
      <p class="address__pin">ул. В. Хромых, д. 29, 2 эт, оф. No2</p>
    </div>
    <form class="address__form address-form" action="/" method="post">
      <p class="address-form__title">Запишитесь на консультацию<br> по сделке с ипотекой</p>
      <label>
        <input class="address-form__input" type="text" placeholder="+7 (___) __-__-___">
      </label>
      <button class="address-form__submit" type="submit">Получить консультацию</button>
    </form>
  </section>
</template>

<style lang="scss">
.address {
  display: flex;
  flex-direction: column;
  padding: 50px 25px 0;
  background-image: url("../images/we-on-map.jpg");
  background-repeat: no-repeat;
  background-position: 100% 100%;

  @media (min-width: 1440px) {
    padding-top: 170px;
    background-image: url("../images/we-on-map-desktop.jpg");
    background-position: 100% 145%;
  }
}

.address__o {
  margin-bottom: 5px;
  font-size: 24px;
  line-height: 120%;
  font-weight: 900;
  color: #35465e;
  text-align: center;

  @media (min-width: 1440px) {
    font-size: 36px;
    margin-bottom: 22px;
  }
}

.address__pin {
  padding-bottom: 500px;
  font-size: 16px;
  line-height: 120%;
  font-weight: 200;
  text-align: center;
  color: #35465e;

  @media (min-width: 1440px) {
    font-size: 25px;
    padding-bottom: 618px;
  }
}

.address__form {
  width: 270px;
  padding: 23px 13px 26px;
  box-sizing: border-box;
  background-color: #f2f2f2;
  border-radius: 5px;
  position: relative;
  top: 57px;

  @media (min-width: 1440px) {
    width: 950px;
    height: 145px;
    margin: 0 auto;
    top: 0;
    color: #ebebeb;
    display: flex;
    padding: 42px 62px 42px 54px;
    position: relative;
    z-index: 10;
  }
}

.address-form__title {
  margin-bottom: 31px;
  font-size: 16px;
  line-height: 120%;
  font-weight: 900;
  text-align: center;
  color: #35465e;

  @media (min-width: 1440px) {
    font-size: 20px;
    text-align: left;
    margin: 0;
    margin-right: 63px;
  }
}

.address-form__input {
  width: 243px;
  height: 57px;
  margin-bottom: 20px;
  padding: 7px 15px;
  box-sizing: border-box;
  border: none;
  border-radius: 5px;
}

.address-form__submit {
  width: 242px;
  height: 49px;
  border: none;
  background-color: #2489ff;
  border-radius: 5px;
  font-size: 16px;
  line-height: 120%;
  color: #ebebeb;
  font-family: "Roboto", "Arial", sans-serif;
  cursor: pointer;
  box-sizing: border-box;
  padding: 5px 15px;

  @media (min-width: 1440px) {
    width: 216px;
    height: 56px;
    margin-left: 40px;
  }
}
</style>