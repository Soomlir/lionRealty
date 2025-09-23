<script></script>

<template>
  <section class="details">
    <picture>
      <source srcset="/images/details-desktop-1.jpg" width="1146" height="493" media="(min-width: 1440px)">
      <img class="details__image" src="/images/details-mobile-1.jpg" width="270" height="158" alt="Фото дома.">
    </picture>
    <div class="details__info">
      <h3 class="details__heading">Всё, что нужно знать<br class="br-mobile"> об этом доме</h3>
      <p class="details__text">Участок расположен среди виноградников и леса, соседей рядом нет.</p>
      <p class="details__text">Массив находится под охраной фирмы «Безопасный город».<br class="br-desktop">
        Посёлок обеспечен своей трансформаторной подстанцией на
        400 кВт, подведен центральный водопровод плюс дополнительные резервуары с запасом воды
        и каптаж на 120 кубов.
      </p>
    </div>
    <a class="details__more" href="#!">Читать полностью</a>
  </section>
</template>

<style lang="scss">
.details {
  width: 270px;
  margin: 0 auto;
  padding-top: 50px;
  padding-bottom: 100px;

  @media (min-width: 1440px) {
    width: 1146px;
    margin: 0 auto;
  }
}

.details__image {
  margin-bottom: 35px;

  @media (min-width: 1440px) {
    margin-bottom: 69px;
  }
}

.details__heading {
  margin-bottom: 20px;
  font-weight: 900;
  font-size: 24px;
  line-height: 120%;

  @media (min-width: 1440px) {
    margin-bottom: 28px;
    font-size: 36px;
    color: #35465e;
  }
}

.details__text {
  margin-bottom: 35px;
  font-weight: 200;
  font-size: 14px;
  line-height: 120%;

  @media (min-width: 1440px) {
    font-size: 16px;
    width: 590px;
    margin-bottom: 47px;
  }
}

.details__more {
  display: block;
  width: 226px;
  height: 49px;

  padding: 15px 20px;
  padding-left: 40px;
  text-align: center;
  color: #ebebeb;
  font-size: 16px;
  line-height: 20px;
  font-family: "Roboto", "Arial", sans-serif;
  background-color: #2489ff;
  border-radius: 5px;
  position: relative;
  box-sizing: border-box;

  &::before {
    position: absolute;
    content: "";
    top: 16px;
    left: 32px;
    width: 15px;
    height: 18px;
    background-image: url("../images/book.svg");
  }

  @media (min-width: 1440px) {
    width: 235px;
    height: 66px;
    padding: 23px 20px;
    padding-left: 40px;

    &::before {
      top: 25px;
      left: 40px;
    }
  }
}
</style>