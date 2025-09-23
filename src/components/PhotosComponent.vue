<script></script>

<template>
  <section class="photos">
    <h2 class="photos__heading">Фотографии объекта</h2>
    <ul class="photos__list">
      <li class="photos__item photos__item--1">
        <a href="#!" class="photos__link photos__link--1">
          <picture>
            <source srcset="/images/photos-desktop-1.jpg" width="753" height="576" media="(min-width: 1440px)">
            <img class="photos__image photos__image--1" src="/images/photos-1.jpg" width="270" height="200"
              alt="Фото объекта.">
          </picture>
        </a>
      </li>
      <li class="photos__item photos__item--2">
        <a href="#!" class="photos__link photos__link--2">
          <picture>
            <source srcset="/images/photos-desktop-2.jpg" width="362" height="271" media="(min-width: 1440px)">
            <img class="photos__image photos__image--2" src="/images/photos-2.jpg" width="270" height="200"
              alt="Фото объекта.">
          </picture>
        </a>
      </li>
      <li class="photos__item photos__item--3">
        <a href="#!" class="photos__link photos__link--3">
          <picture>
            <source srcset="/images/photos-desktop-3.jpg" width="362" height="271" media="(min-width: 1440px)">
            <img class="photos__image photos__image--3" src="/images/photos-3.jpg" width="270" height="200"
              alt="Фото объекта.">
          </picture>
        </a>
      </li>
      <li class="photos__item photos__item--4">
        <a href="#!" class="photos__link photos__link--4">
          <picture>
            <source srcset="/images/photos-desktop-4.jpg" width="362" height="271" media="(min-width: 1440px)">
            <img class="photos__image photos__image--4" src="/images/photos-4.jpg" width="270" height="200"
              alt="Фото объекта.">
          </picture>
        </a>
      </li>
      <li class="photos__item photos__item--5">
        <a href="#!" class="photos__link photos__link--5">
          <picture>
            <source srcset="/images/photos-desktop-5.jpg" width="754" height="577" media="(min-width: 1440px)">
            <img class="photos__image photos__image--5" src="/images/photos-5.jpg" width="270" height="200"
              alt="Фото объекта.">
          </picture>
        </a>
      </li>
      <li class="photos__item photos__item--6">
        <a href="#!" class="photos__link photos__link--6">
          <picture>
            <source srcset="/images/photos-desktop-6.jpg" width="362" height="271" media="(min-width: 1440px)">
            <img class="photos__image photos__image--6" src="/images/photos-6.jpg" width="270" height="200"
              alt="Фото объекта.">
          </picture>
        </a>
      </li>
    </ul>
    <a class="photos__more" href="#!">Больше фото</a>
  </section>
</template>

<style lang="scss">
.photos {
  padding: 50px 30px 100px;

  @media (min-width: 1440px) {
    padding: 72px 147px 100px;
  }
}

.photos__heading {
  margin-bottom: 40px;
  font-size: 24px;
  line-height: 30px;
  text-align: center;

  @media (min-width: 1440px) {
    text-align: left;
    font-size: 36px;
    line-height: 36px;
  }
}

.photos__list {
  display: flex;
  flex-direction: column;
  gap: 20px;
  margin-bottom: 40px;

  @media (min-width: 1440px) {
    display: grid;
    grid-template-columns: repeat(3, 362px);
    grid-template-rows: repeat(4, auto);
    gap: 36px 30px;
    margin-bottom: 47px;
  }
}

.photos__item {
  @media (min-width: 1440px) {
    &--1 {
      grid-column: span 2;
      grid-row: span 2;
    }

    &--3 {
      grid-row: 2;
      grid-column: 3;
    }

    &--5 {
      grid-row: 3 / -1;
      grid-column: 2 / -1;
    }
  }
}

.photos__more {
  font-size: 16px;
  line-height: 24px;
  color: #35465e;
  position: relative;
  padding-left: 48px;
  width: 100px;
  margin: 0 auto;
  display: block;

  &::before {
    position: absolute;
    content: "";
    top: 0;
    left: 0;
    width: 24px;
    height: 24px;
    background-image: url("../images/more.svg");
  }
}
</style>