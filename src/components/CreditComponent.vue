<script></script>

<template>
  <section class="credit">
    <div class="credit__wrap">
      <h2 class="visually-hidden">Подробности ипотеки</h2>
      <p class="credit__title">Этот объект можно<br class="br-desktop"> оформить в ипотеку</p>
      <div class="credit__variants variants">
        <a class="variants__link" href="#!">Стандартная ипотека</a>
        <a class="variants__link" href="#!">Военная ипотека</a>
        <a class="variants__link" href="#!">Материнский капитал</a>
      </div>
      <p class="variants__heading">Сопровождаем сделку<br class="br-mobile"> на всех этапах</p>
      <p class="variants__text">Если вам одобрили ипотеку, мы подготовим все нужные документы для банка,
        поможем с заключением сделки и безопасным оформлением имущества на вас</p>
    </div>
    <form class="variants__form" action="/" method="post">
      <p class="form__title">Запишитесь на консультацию<br> по сделке с ипотекой</p>
      <label>
        <input class="form__input" type="text" placeholder="+7 (___) __-__-___">
      </label>
      <button class="form__submit" type="submit">Получить консультацию</button>
    </form>
  </section>
</template>

<style lang="scss">
.credit {
  width: 306px;
  margin: 0 auto;
  padding: 30px 18px;
  box-sizing: border-box;

  @media (min-width: 1440px) {
    display: flex;
    justify-content: space-between;
    width: 1146px;
    height: 536px;
    margin: 0 auto;
    margin-top: 67px;
    padding: 87px 76px 116px 98px;
    box-shadow: 0 -8px 14px rgba(#35465e, 0.02),
      0 50px 80px rgba(#35465e, 0.1);
  }
}

.credit__title {
  margin-bottom: 25px;
  font-size: 24px;
  line-height: 120%;
  font-weight: 900;

  @media (min-width: 1440px) {
    font-size: 36px;
    color: #35465e;
  }
}

.variants {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-bottom: 23px;
}

.variants__link {
  font-size: 10px;
  line-height: 13px;
  color: #35465e;
  display: flex;
  padding: 7px 10px;
  background-color: #f2f2f2;

  @media (min-width: 1440px) {
    font-size: 14px;
    padding: 15px 10px;
  }
}

.variants__heading {
  margin-bottom: 15px;
  font-size: 18px;
  line-height: 120%;
  color: #35465e;
  font-weight: 700;
}

.variants__text {
  width: 242px;
  margin-bottom: 35px;
  font-weight: 200;
  font-size: 14px;
  line-height: 120%;

  @media (min-width: 1440px) {
    width: 422px;
    font-size: 20px;
  }
}

.variants__form {
  width: 270px;
  padding: 23px 13px 26px;
  box-sizing: border-box;
  background-color: #f2f2f2;
  border-radius: 5px;

  @media (min-width: 1440px) {
    width: 400px;
    padding: 50px;
  }
}

.form__title {
  margin-bottom: 31px;
  font-size: 16px;
  line-height: 120%;
  font-weight: 900;
  text-align: center;
  color: #35465e;

  @media (min-width: 1440px) {
    font-size: 22px;
  }
}

.form__input {
  width: 243px;
  height: 57px;
  margin-bottom: 20px;
  padding: 7px 15px;
  box-sizing: border-box;
  border: none;
  border-radius: 5px;

  @media (min-width: 1440px) {
    width: 300px;
    font-size: 16px;
  }
}

.form__submit {
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
    width: 300px;
    height: 66px;
  }
}
</style>