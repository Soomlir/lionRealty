<script></script>

<template>
  <section class="about">
    <a class="about__navigation" href="#!">&larr; в каталог</a>
    <h1 class="about__heading">Дом 100 м<sup>2</sup> под Алуштой<br class="br-desktop"> на участке 50 соток</h1>
    <ul class="about__list">
      <li class="about__item">
        <p class="about__value">100 000 000 ₽</p>
        <p class="about__title">Цена объекта</p>
      </li>
      <li class="about__item">
        <p class="about__value">100 м<sup>2</sup></p>
        <p class="about__title">Площадь дома</p>
      </li>
      <li class="about__item about__item--price">
        <p class="about__value">1 000 000 ₽</p>
        <p class="about__title">Цена 1 кв. м.</p>
      </li>
      <li class="about__item">
        <p class="about__value">50 соток</p>
        <p class="about__title">Площадь участка</p>
      </li>
    </ul>

    <div class="about__tags tags">
      <a class="tags__link" href="#!">Частное домовладение</a>
      <a class="tags__link" href="#!">Удобный подъезд</a>
      <a class="tags__link" href="#!">Современная архитектура</a>
      <a class="tags__link" href="#!">Готово для проживания</a>
      <a class="tags__link" href="#!">Живописный вид на море</a>
      <a class="tags__link" href="#!">Закрытая территория</a>
    </div>

    <div class="tags__links-wrap">
      <a class="about__link-map" href="#!">Посмотреть на карте</a>
      <a class="about__link-object" href="#!">Подробнее об объекте</a>
    </div>
    <a class="about__play" href="#!">
      <span class="visually-hidden">Проиграть.</span>
      <img src="/images/play-button.svg" width="145" height="145" alt="Проиграть.">
    </a>
  </section>
</template>

<style lang="scss">
.about {
  @media (min-width: 1440px) {
    position: relative;
    padding-top: 72px;
  }
}

.about__navigation {
  display: block;
  margin-bottom: 30px;
  font-size: 16px;
  line-height: 20px;
  color: #ffffff;
  text-decoration: none;
  position: relative;

  &::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
  }

  @media (min-width: 1440px) {
    font-size: 26px;
    line-height: 26px;
  }
}

.about__heading {
  margin-bottom: 40px;
  font-size: 20px;
  line-height: 24px;
  color: #ffffff;

  sup {
    font-size: 11px;
    line-height: 11px;
  }

  @media (min-width: 1440px) {
    font-size: 58px;
    line-height: 64px;

    sup {
      font-size: 30px;
      line-height: 30px;
    }
  }
}

.about__list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-bottom: 40px;
}

.about__item {
  width: 120px;

  @media (min-width: 1440px) {
    width: 154px;

    &:first-child {
      order: -2;
    }

    &--price {
      order: -1;
    }
  }
}

.about__value {
  margin-bottom: 9px;
  font-size: 18px;
  line-height: 24px;
  color: #ffffff;
  font-weight: 700;

  sup {
    font-size: 11px;
    line-height: 11px;
  }

  @media (min-width: 1440px) {
    font-size: 24px;
  }
}

.about__title {
  font-size: 15px;
  line-height: 20px;
  color: #ffffff;
}

.tags {
  display: flex;
  flex-wrap: wrap;
  column-gap: 5px;
  row-gap: 10px;
  padding-bottom: 50px;

  @media (min-width: 1440px) {
    width: 526px;
  }
}

.tags__link {
  display: flex;
  padding: 5px 7px;
  font-size: 10px;
  line-height: 10px;
  color: #000000;
  text-decoration: none;
  background-color: #F2F2F2;
  border-radius: 5px;

  @media (min-width: 1440px) {
    padding: 5px 10px;
    font-size: 14px;
    line-height: 24px;
  }
}

.tags__links-wrap {
  display: contents;

  @media (min-width: 1440px) {
    display: flex;
    align-items: center;
  }
}

.about__link-map {
  display: block;
  width: 260px;
  height: 61px;
  margin-bottom: 28px;
  box-sizing: border-box;
  background-color: #2489FF;
  padding: 20px 40px 20px 80px;
  position: relative;
  border-radius: 49px;
  color: #ffffff;
  text-decoration: none;
  font-size: 15px;
  line-height: 20px;

  &::before {
    content: "";
    position: absolute;
    top: 3px;
    left: 3px;
    width: 55px;
    height: 55px;
    border-radius: 50%;
    background-image: url("../images/map-link.jpg");
  }
}

.about__link-object {
  display: block;
  text-align: center;
  font-size: 16px;
  line-height: 20px;
  color: #ffffff;
  text-decoration: none;
  position: relative;
  padding-bottom: 50px;

  &::before {
    position: absolute;
    content: "";
    width: 9px;
    height: 9px;
    top: 6px;
    left: 30px;
    background-image: url("../images/arrow-down.svg");
    background-repeat: no-repeat;
  }

  @media (min-width: 1440px) {
    padding-bottom: 25px;
    padding-left: 74px;

    &::before {
      width: 12px;
      height: 12px;
      left: 59px;
    }
  }
}

.about__play {
  width: 145px;
  height: 145px;
  margin: 0 auto;
  display: block;

  @media (min-width: 1440px) {
    position: absolute;
    top: 232px;
    right: 109px;

    img {
      width: 194px;
      height: 194px;
    }
  }
}
</style>