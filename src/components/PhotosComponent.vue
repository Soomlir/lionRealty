<script></script>

<template>
  <section class="photos">
    <h2 class="photos__heading">Фотографии объекта</h2>
    <ul class="photos__list">
      <li class="photos__item">
        <a href="#!" class="photos__link">
          <img src="/images/photos-1.jpg" width="270" height="200" alt="Фото объекта.">
        </a>
      </li>
      <li class="photos__item">
        <a href="#!" class="photos__link">
          <img src="/images/photos-2.jpg" width="270" height="200" alt="Фото объекта.">
        </a>
      </li>
      <li class="photos__item">
        <a href="#!" class="photos__link">
          <img src="/images/photos-3.jpg" width="270" height="200" alt="Фото объекта.">
        </a>
      </li>
      <li class="photos__item">
        <a href="#!" class="photos__link">
          <img src="/images/photos-4.jpg" width="270" height="200" alt="Фото объекта.">
        </a>
      </li>
      <li class="photos__item">
        <a href="#!" class="photos__link">
          <img src="/images/photos-5.jpg" width="270" height="200" alt="Фото объекта.">
        </a>
      </li>
      <li class="photos__item">
        <a href="#!" class="photos__link">
          <img src="/images/photos-6.jpg" width="270" height="200" alt="Фото объекта.">
        </a>
      </li>
    </ul>
    <a class="photos__more" href="#!">Больше фото</a>
  </section>
</template>

<style lang="scss">
.photos {
  padding: 50px 30px 100px;
}

.photos__heading {
  margin-bottom: 40px;
  font-size: 24px;
  line-height: 30px;
  text-align: center;
}

.photos__list {
  display: flex;
  flex-direction: column;
  gap: 20px;
  margin-bottom: 40px;
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