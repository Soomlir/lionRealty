<script></script>

<template>
  <header class="header">
    <div class="header__menu">
      <a href="#!">
        <div class="header__gamburger">
          <span></span>
          <span></span>
          <span></span>
        </div>
        <span class="header__menu-title">Меню</span>
      </a>
    </div>
    <a class="header__logo" href="#!">
      <img src="/images/logo-mobile.svg" width="30" height="48" alt="Логотип сайта Lion Realty.">
    </a>
    <ul class="header__list">
      <li class="header__item">
        <a class="header__link header__link--viber" href="#!">
          <span class=visually-hidden>Viber.</span>
        </a>
      </li>
      <li class="header__item">
        <a class="header__link header__link--whatsup" href="#!">
          <span class=visually-hidden>Whats up.</span>
        </a>
      </li>
      <li class="header__item">
        <a class="header__link header__link--telegram" href="#!">
          <span class=visually-hidden>Telegram.</span>
        </a>
      </li>
    </ul>
    <a class="header__phone" href="tel:+79788881654">+7 (978) 888-1-654</a>
  </header>
</template>

<style lang="scss">
.header {
  display: flex;
  align-items: center;
  padding-top: 28px;
  padding-bottom: 20px;

  @media (min-width: 1440px) {
    padding-top: 39px;
  }
}

.header__menu {
  width: 76px;
  height: 19px;
  margin-right: 42px;

  a {
    display: flex;
    align-items: center;
    gap: 11px;
  }
}

.header__menu-title {
  text-decoration: none;
  font-size: 16px;
  line-height: 20px;
  color: #ffffff;
}

.header__gamburger {
  span {
    display: block;
    width: 20px;
    height: 1px;
    background-color: #ffffff;
    margin-bottom: 3px;
  }

  span:last-child {
    width: 14px;
  }

}

.header__logo {
  margin-right: auto;

  @media (min-width: 1440px) {
    margin-left: 431px;

    img {
      width: 48px;
      height: 76px;
    }
  }
}

.header__list {
  display: flex;
}

.header__link {
  display: flex;
  align-items: center;
  justify-content: center;
  background-repeat: no-repeat;
  width: 17px;
  height: 17px;
  margin-left: 13px;

  &--viber {
    background-image: url("../images/social-viber.svg");
  }

  &--whatsup {
    background-image: url("../images/social-whatsup.svg");
  }

  &--telegram {
    background-image: url("../images/social-telegram.svg");
  }

  @media (min-width: 1440px) {
    width: 20px;
    height: 20px;

    background-size: 20px 20px;
  }
}

.header__phone {
  display: none;

  @media (min-width: 1440px) {
    display: block;
    margin-left: 20px;
    font-size: 16px;
    line-height: 20px;
    color: #ffffff;
  }
}
</style>