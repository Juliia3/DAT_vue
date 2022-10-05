<script setup>
import { RouterLink, RouterView } from 'vue-router';
import './components/Header/header.scss';
import './assets/styles/index.scss'

</script>

<template>
  <div class="page-wrapper">
    <header class="menu">
      <div class="menu__container container">
        <nav class="menu__nav">
          <ul class="menu__list">
            <li class="menu__item header"><a class="menu__link" target="_blank" href="">
                <RouterLink to="/about" target="_blank">Про нас</RouterLink>
                <!-- <img class="menu__vector vector" src="@/assets/img/vector.svg" alt="vector">-->
              </a>
            </li>
            <li class="menu__item header">
              <a class="menu__link" href="">
                <RouterLink to="/catalog" target="_blank">Каталог продукції</RouterLink>
              </a>
            </li>
            <li class="menu__item header">
              <a class="menu__link" href="">
                <RouterLink to="/pay" target="_blank">Оплата і доставка</RouterLink>
              </a>
            </li>
            <li class="menu__item header">
              <a class="menu__link" href="">Партнери</a>
            </li>
            <li class="menu__item header">
              <a class="menu__link" href="">Новини</a>
            </li>
            <li class="menu__item header">
              <a class="menu__link" href="">Контакти</a>
            </li>
          </ul>
        </nav>
        <img class="menu__line line" src="@/assets/img/line.svg" alt="line">
        <p class="menu__reg header"><a class="menu__log-link" href="">
            <img class="menu__login-img" src="@/assets/img/login.svg" alt="login"> <span class="menu__login">Вхід
              |</span>
            <span class="menu__login">Реєстрація</span></a></p>
      </div>
    </header>
    <RouterLink to="/home">Home</RouterLink>
    <RouterView />
    <footer class="footer">
      <div class="footer__container container">
        <div class="footer__menu">
          <div class="footer__logo-box">
            <router-link to="/" target= '_blank'><img class="search__logo logo" src="@/assets/img/logo.png" alt="logo"></router-link>
            <p class="footer__text text">
              Пропонуємо покупцям широкий вибір насіння овочів
            </p>
          </div>
          <nav class="footer__nav">
            <ul class="footer__list p">
              <li class="footer__item">
                <p class="footer__item-name">
                  <a class="footer__link" href="">Інформація</a>
                </p>
                <div class="footer__item-info-block">
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Про компанію</a>
                  </p>
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Оплата і доставка</a>
                  </p>
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Партнери</a>
                  </p>
                </div>
              </li>
              <li class="footer__item">
                <p class="footer__item-name">
                  <a class="footer__link" href="">Товари</a>
                </p>
                <div class="footer__item-info-block">
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Каталог продукції</a>
                  </p>
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Засоби захисту рослин</a>
                  </p>
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Насіння</a>
                  </p>
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Добрива</a>
                  </p>
                  <p class="footer__item-info">
                    <a class="footer__link" href="">Агроному в поміч</a>
                  </p>
                </div>
              </li>
              <li class="footer__item">
                <p class="footer__item-name">
                  <a class="footer__link" href="">Контакти</a>
                </p>
                <div class="footer__item-info-block">
                  <div class="search__contact footer__item-info">
                    <div class="search__phone-box">
                      <div class="search__phone-icon-box">
                        <a class="search__phone-link" href=""><img class="search__phone-icon icon"
                            src="@/assets/img/phone.svg" alt=""></a>
                      </div>
                      <div class="search__phone-contacts">
                        <p class="search__number number text">+38 (067) 115 00 58</p>
                        <p class="search__text call"><a class="search__call" href="">Замовити
                            зворотній
                            зв’язок</a>
                        </p>
                      </div>
                    </div>
                  </div>
                  <div class="search__contact footer__item-info">
                    <div class="search__phone-box">
                      <div class="search__phone-icon-box">
                        <a class="search__phone-link" href=""><img class="search__phone-icon icon"
                            src="@/assets/img/email.svg" alt=""></a>
                      </div>
                      <div class="search__phone-contacts">
                        <p class="search__number email text">DAT@gmail.com</p>
                      </div>
                    </div>
                  </div>
                </div>
              </li>
            </ul>
          </nav>
        </div>
        <div class="footer__end">
          <img class="footer__line" src="@/assets/img/footer-line.svg" alt="line">
          <p class="footer__date name">© 2022 DAT</p>
        </div>
      </div>
    </footer>
  </div>

</template>
