<script></script>

<template>
  <section class="address">
    <h2 class="visually-hidden">Наше расположение</h2>
    <div class="address__wrap">
      <p class="address__o">Объект находится<br> по адресу</p>
      <p class="address__pin">ул. В. Хромых, д. 29, 2 эт, оф. No2</p>
    </div>
    <form class="variants__form form" action="/" method="post">
      <p class="form__title">Запишитесь на консультацию<br> по сделке с ипотекой</p>
      <label>
        <input class="form__input" type="text" placeholder="+7 (___) __-__-___">
      </label>
      <button class="form__submit" type="submit">Получить консультацию</button>
    </form>
  </section>
</template>

<style>
.address {
  display: flex;
  flex-direction: column;
  padding: 50px 25px 0;
  background-image: url("../images/we-on-map.jpg");
  background-repeat: no-repeat;
  background-position: 100% 100%;
}

.address__o {
  margin-bottom: 5px;
  font-size: 24px;
  line-height: 120%;
  font-weight: 900;
  color: #35465e;
  text-align: center;
}

.address__pin {
  padding-bottom: 500px;
  font-size: 16px;
  line-height: 120%;
  font-weight: 200;
  text-align: center;
  color: #35465e;
}

.variants__form {
  position: relative;
  top: 57px;
}
</style>