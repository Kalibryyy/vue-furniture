<template>
  <header class="header">
    <div class="header__container">
      <div class="header__contacts">
        <ul class="header__contacts-list">
          <li class="header__contacts-item">
            <img
              class="header__contacts-icon"
              src="~static/images/mail.svg"
              alt="иконка почтового ящика"
            />
            <p class="header__contact-text">mebel@mail.ru</p>
          </li>
          <li class="header__contacts-item">
            <img
              class="header__contacts-icon"
              src="~static/images/location.svg"
              alt="иконка местоположения"
            />
            <p class="header__contact-text">
              Санкт-Петербург, ул. Ленина, д. 1
            </p>
          </li>
          <li class="header__contacts-item">
            <img
              class="header__contacts-icon"
              src="~static/images/phone.svg"
              alt="иконка телефона"
            />
            <p class="header__contact-text">+ 7 911 985 98 22</p>
          </li>
        </ul>
      </div>
      <div class="header__wrapper">
        <div class="logo"></div>
        <div class="header__catalog">
          <img
            class="header__catalog-icon"
            src="~static/images/menu.svg"
            alt="иконка меню"
          />
          <p class="header__catalog-text">Каталог</p>
        </div>
        <form class="header__form">
          <input type="text" class="header__input" />
          <img
            src="~static/images/search.svg"
            alt="иконка поиска"
            class="header__search-img"
          />
        </form>
        <div class="header__options-item">
          <img src="~static/images/payment.svg" alt="картинка оплаты" />
          <p class="header__options-text">Оплата</p>
        </div>
        <div class="header__options-item">
          <img src="~static/images/delivery.svg" alt="картинка доставки" />
          <p class="header__options-text">Доставка</p>
        </div>
        <div class="header__options-item">
          <img src="~static/images/like.svg" alt="картинка сердечка" />
          <p class="header__options-text">Доставка</p>
        </div>
      </div>
      <nav class="navigation">
        <ul class="navigation__list">
          <li class="navigation__item">Акции и скидки</li>
          <li class="navigation__item">Кухни</li>
          <li class="navigation__item">Детские</li>
          <li class="navigation__item">Спальни</li>
          <li class="navigation__item">Корпусная мебель</li>
          <li class="navigation__item">Офисная мебель</li>
          <li class="navigation__item">Торговое оборудование</li>
          <li class="navigation__item">Услуги</li>
          <li class="navigation__item">Статьи</li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
.header__container {
  margin: 0 auto;
}
.header__contacts {
  background-color: #c9d6a4;
  padding: 0 250px;
}

@media screen and (max-width: 1440px) {
  .header__contacts {
    padding-left: 50px;
    padding-right: 50px;
  }
}

.header__contacts-list {
  list-style-type: none;
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-end;
  padding: 0;
  margin: 0;
  align-items: center;
  min-height: 53px;
  padding: 10px 0;
  box-sizing: border-box;
}

.header__contacts-item {
  display: flex;
  margin: 0 60px 10px 0;
}

@media screen and (max-width: 1280px) {
  .header__contacts-item {
    margin-right: 10px;
  }
}

.header__contacts-icon {
  height: 30px;
  width: 30px;
  margin-right: 10px;
}

@media screen and (max-width: 1280px) {
  .header__contacts-icon {
    height: 20px;
    width: 20px;
    margin-right: 5px;
  }
}

.header__contact-text {
  margin: 0;
  align-self: center;
  font-size: 20px;
  line-height: 1.75;
  font-weight: 400;
  font-family: "Open Sans", sans-serif;
  color: #494949;
}

@media screen and (max-width: 1280px) {
  .header__contact-text {
    font-size: 16px;
    line-height: 1.3;
    font-weight: 400;
  }
}

.header__wrapper {
  display: flex;
  justify-content: space-between;
  padding: 30px 0 35px 0;
  box-sizing: border-box;
}

.header__catalog {
  display: flex;
  align-items: center;
  border: 2px solid rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  height: 50px;
  min-width: 180px;
}

.header__catalog-icon {
  width: 35px;
  height: 25px;
  margin: 0 20px 0 14px;
}

.header__catalog-text {
  margin: 0;
  align-self: center;
  font-size: 20px;
  line-height: 1.75;
  font-weight: 400;
  font-family: "Open Sans", sans-serif;
  color: #494949;
  text-transform: uppercase;
}

@media screen and (max-width: 1280px) {
  .header__catalog-text {
    font-size: 16px;
    line-height: 1.3;
    font-weight: 400;
  }
}

.header__form {
  /* width: 100%; */
  height: 50px;
  border: 2px solid rgba(0, 0, 0, 0.1);
  border-radius: 10px;
  display: flex;
  align-items: center;
}

.header__input {
  width: 100%;
  height: 100%;
  background-color: transparent;
  font-family: "Open Sans", sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 22px;
  color: #494949;
  border: none;
  padding: 8px 20px;
  box-sizing: border-box;
}

.header__input:focus {
  outline: none;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.header__search-img {
  width: 28px;
  height: 28px;
  margin: 0 10px;
}

.logo {
  background-image: url("~static/images/logo.png");
  width: 110px;
  height: 130px;
  margin-top: -60px;
}

.navigation__list {
  list-style-type: none;
  padding: 0;
  margin: 0 0 50px 0;
  display: flex;
  justify-content: space-between;
}

.navigation__item {
  text-transform: uppercase;
}
</style>
