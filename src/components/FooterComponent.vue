<script></script>

<template>
  <footer class="footer">
    <a class="footer__logo-link" href="#!">
      <img src="/images/footer-logo-mobile.svg" alt="Логотип сайта.">
    </a>
    <a class="footer__tel" href="tel:+79788881654">+7 (978) 888-1-654</a>
    <ul class="footer__list">
      <li class="footer__item">
        <a class="footer__link footer__link--viber" href="#!">
          <span class=visually-hidden>Viber.</span>
        </a>
      </li>
      <li class="footer__item">
        <a class="footer__link footer__link--whatsup" href="#!">
          <span class=visually-hidden>Whats up.</span>
        </a>
      </li>
      <li class="footer__item">
        <a class="footer__link footer__link--telegram" href="#!">
          <span class=visually-hidden>Telegram.</span>
        </a>
      </li>
    </ul>
    <p class="footer__atention">сайт носит исключительно информационный характер
      и ни при каких условиях не является публичной офертой</p>
  </footer>
</template>

<style lang="scss">
.footer {
  padding: 280px 67px 331px;
  background-color: #3053b5;
  background-image: url("../images/our-office-mobile.png");
  background-position: 100% 100%;
  background-repeat: no-repeat;
}

.footer__logo-link {
  display: block;
  margin-bottom: 27px;
}

.footer__tel {
  display: block;
  margin-bottom: 10px;
  color: #ffffff;
  font-size: 22px;
  line-height: 120%;
  font-weight: 200;
}

.footer__list {
  display: flex;
  margin: 0 auto;
  width: 100px;
  margin-bottom: 27px;
}

.footer__link {
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
}

.footer__atention {
  font-size: 14px;
  line-height: 120%;
  font-weight: 200;
  color: #ffffff;
}
</style>