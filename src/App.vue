<template>
  <header>
    <div class="logo"></div>
    <nav>
      <router-link to="/">Репродукции</router-link>
      <router-link to="/about">Новинки</router-link>
      <router-link to="/login">Всё о нас</router-link>
    </nav>
  </header>
  <main>
    <BigItem></BigItem>
    <FilterLine></FilterLine>
    <div class="frame">
      <div v-for="cart in france" :key="cart.id">
        <ItemCard :name_artist="cart.name_artist" :name_picture="cart.name_picture" :material="cart.material"
          :price="cart.price" :url="cart.url">
        </ItemCard>
      </div>
    </div>
  </main>
  <PromoItem></PromoItem>
  <footer>

    <div id="ref">
      <div id="ref_1">
        <div id="logo_phone">
          <img class="footer_logo" src="./assets/incHouse.png" alt="">

        </div>
        <div class="break break1"></div>
        <div id="footer_phone">
          <p>+7 (999) 543-54-54</p>
          <p>Мастерская</p>
        </div>
        <div class="break break2"></div>
        <div id="rep">
          <p>Репродукции</p>
          <a href="">Франция</a>
          <a href="">Германия</a>
          <a href="">Англия</a>
        </div>
        <div id="new">
          <p>Новинки</p>
          <a href="">2021</a>
          <a href="">2020</a>
        </div>
        <div id="us_about">
          <p>О нас</p>
          <a href="">Художники</a>
          <a href="">Менеджеры</a>
        </div>
        <div class="break break1"></div>
        <div id="ref_2">
          <img class="ms" src="./assets/ms.png" align="left" alt="">
          <p>Ink. House ®</p>
          <p>All rights reserved</p>
        </div>
      </div>
      
    </div>
  </footer>
</template>

<script>
import BigItem from './components/BigItem.vue';
import FilterLine from './components/FilterLine.vue';
import ItemCard from './components/ItemCard.vue';
import PromoItem from './components/PromoItem.vue';
export default {
  name: "App",
  data() {
    return {
      france: [
        {
          id: 1,
          name_artist: "Марсель Руссо",
          name_picture: "Охота Амура",
          material: "Холст, масло (50x80)",
          price: "14 500 руб",
          url: "01.jpg"
        },
        {
          id: 2,
          name_artist: "Анри Селин",
          name_picture: "Дама с собачкой",
          material: "Акрил, бумага (50x80)",
          price: "16 500 руб",
          url: "02.jpg"
        },
        {
          id: 3,
          name_artist: "Франсуа Дюпон",
          name_picture: "Процедура",
          material: "Цветная литография (40x60)",
          price: "20 000 руб",
          url: "03.jpg"
        },
        {
          id: 4,
          name_artist: "Луи Детуш",
          name_picture: "Роза",
          material: "Бумага, акрил (50x80)",
          price: "12 000 руб",
          url: "04.jpg"
        },
        {
          id: 5,
          name_artist: "Франсуа Дюпон",
          name_picture: "Птичья трапеза",
          material: "Цветная литография (40x60)",
          price: "22 500 руб",
          url: "05.jpg"
        },
        {
          id: 6,
          name_artist: "Пьер Моранж",
          name_picture: "Пейзаж с рыбой",
          material: "Цветная литография (40x60)",
          price: "20 000 руб",
          url: "06.jpg"
        }
      ],
    }
  },
  components: {
    BigItem,
    FilterLine,
    ItemCard,
    PromoItem
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.break{
  flex-basis: 100%;
  height: 0;
}

.break1{
  display: none;
}

#ref_1 {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
@media screen and (max-width: 2440px) {
  main {
    padding: 0% 13% 0% 13%;
  }

  nav {
    position: absolute;
    right: 13%;
    top: 12pt;
    width: 400pt;
  }

  nav a {
    padding: 0% 0% 0% 15%;
  }

  header {
    padding: 20pt 0% 20pt 0%;
    margin: 0% 0% 0% 0%;
    display: flex;
    background-color: #e1ede6;
  }

  .logo {
    position: absolute;
    width: 200px;
    height: 100px;
    left: 13%;
    top: 5.5pt;
  }

  .frame div:not(.chue, .text_card) {
    width: 31.5%;
  }

  footer {
    display: flex;
    padding: 0% 13% 0% 13%;
    justify-content: space-between;
  }

  #ref {
    display: flex;
    justify-content: right;
  }

 
  #ref_2 {
    display: flex;
    flex-direction: column;
    max-width: 13%;
  }

  #ref_2 p {
    text-align: left;
  }
  
  #rep, #new, #us_about {
    margin-right: 6%;
  }
}

@media screen and (max-width: 998px) {
  main {
    padding: 0% 7% 0% 7%;
  }

  nav {
    position: absolute;
    right: 3%;
    top: 12pt;
    width: 400pt;
  }

  nav a {
    padding: 0% 0% 0% 15%;
  }

  header {
    padding: 20pt 0% 20pt 0%;
    margin: 0% 0% 0% 0%;
    display: flex;
    background-color: #e1ede6;
  }

  .logo {
    position: absolute;
    width: 200px;
    height: 100px;
    left: 3%;
    top: 5.5pt;
  }

  .frame div:not(.chue, .text_card) {
    width: 48%;
  }

  footer {
    display: block;
    padding: 0% 7% 0% 7%;
    justify-content: space-between;
  }

 

  #ref {
    display: flex;
    justify-content: space-between;
  }

  #ref_2 {
    display: flex;
    flex-direction: column;
    max-width: 13%;
    margin-left: 0%;
  }

  #ref_2 p {
    text-align: left;
  }

  #ref_1 {
    flex-wrap: wrap;
  }
}

@media screen and (max-width: 768px) {
  main {
    padding: 0% 3% 0% 3%;
  }

  nav {
    position: relative;
    margin: 0% 10% 0% 10%;
    padding-top: 20pt;
    width: 90%;
    right: 0%;
    display: flex;
    justify-content: space-between;
    align-self: center;
    border-top-width: 2px;
    border-top-style: solid;
    border-top-color: lightslategray;
  }

  nav a {
    padding: 0% 0% 0% 0%;
  }

  header {
    padding: 5pt 0% 20pt 0%;
    display: flex;
    flex-direction: column;
    background-color: #e1ede6;
  }

  .logo {
    align-self: center;
    position: relative;
    width: 145px;
    height: 50px;
    left: 0%;
  }

  .frame div:not(.chue, .text_card) {
    width: 48%;
  }

  #ref {
    display: block;
  }

  #ref_1 {
    justify-content: space-around;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    border-bottom-width: 2px;
    border-bottom-style: solid;
    border-bottom-color: lightslategray;
  }

  #ref_2 {
    max-width: 44%;
    margin: auto;
  }

  #ref_2 p {
    text-align: center;
  }
}

@media screen and (max-width: 510px) {
  .break1{display: block;}
  .break2{display: none;}
  .logo {
    align-self: center;
    position: relative;
    width: 145px;
    height: 35px;
    left: 0%;
    padding: 2% 0% 2% 0%;
    top: 13pt
  }

  header {
    background-color: transparent;
    padding: 0% 0% 0% 0%;
  }

  nav {
    position: relative;
    margin: 0% 0% 0% 0%;
    padding: 5% 5% 5% 5%;
    width: 90%;
    right: 0%;
    display: flex;
    justify-content: space-between;
    align-self: center;
    border: none;
    background-color: #e1ede6;
  }

  .frame div:not(.chue, .text_card) {
    width: 97%;
  }

  #rep, #new, #us_about, #footer_phone {
    margin-right: 0%;
    width: 34%;
  }
}

html {
  padding: auto;
}

body {
  padding: 0% 0% 0% 0%;
  margin: 0% 0% 0% 0%;
  background-color: #f4f6f5;
}

header {
  margin: 0% 0% 0% 0%;
}

nav a {
  font-weight: bold;
  color: black;
}

nav a.router-link-exact-active {
  text-decoration: none;
}

nav a:link,
nav a:visited {
  text-decoration: none;
}

nav a:active,
nav a:hover {
  text-decoration: none;
}

.logo {
  background: url(/src/assets/incHouse.png) rgba(0, 0, 0, 0);
  background-repeat: no-repeat;
  background-color: transparent;
}

.frame {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  flex-basis: 33%;
  justify-content: space-between;
}

.frame div:not(.chue, .text_card) {
  margin: 0% 0% 2.5% 0%;
}

footer {
  background-color: #e1ede6;
}

#footer_phone p {
  text-align: left;
  margin: 0% 0% 0% 0%;
}

#ref_1 #new,

#footer_phone :first-child {
  font: lighter 11pt Verdana, sans-serif;
  color: #2c2d35;
}

#footer_phone :last-child {
  font: lighter 11pt Verdana, sans-serif;
  color: #86928b;
}

#rep,
#new,
#us_about {
  display: flex;
  flex-direction: column;
  text-align: left;
}

#ref_1 a:link,
#ref_1 a:visited {
  text-decoration: none;
  color: #86928b;
}

#ref_1 a:active,
#ref_1 a:hover {
  text-decoration: none;
  color: #86928b;
}

#ref_1 p {
  margin-top: 0%;
  margin-bottom: 8%;
}

#ref a {
  margin-bottom: 16%;
}

.ms {
  max-width: 100%;
}

#ref_2 p {
  margin-top: 0%;
  margin-bottom: 0%;
  color: #86928b;
  font: lighter 8pt Verdana, sans-serif;
}
</style>
