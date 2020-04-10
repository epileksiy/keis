<template lang="pug">
div
  .header
    ul.buts
      img(src="../assets/img/LOGO.png" height=70)
      li.buts
        img(src="../assets/img/Header/Vector.png" width=32 height=32)
        a.buts_text Апгрейд
      li.buts
        img(src="../assets/img/Header/Top.png" width=32 height=32)
        a.buts_text Битва за скин
      li.buts
        img(src="../assets/img/Header/Items.png" width=32 height=32)
        a.buts_text Предметы
      li.buts
        img(src="../assets/img/Header/Games.png" width=32 height=32)
        a.buts_text Игры
    .lk
      .user
        img(src="../assets/img/Header/Оформление авы.png")
        .user_info
          a(style="font-weight:300;") Aska.again
          a(style="font-weight:600;") 276.76 ₽
      .lk_but
        a + Пополнить
      img(src="../assets/img/Header/exit.png" width=27 height=27 style="margin-right: 25px;")
  .footer
    .footer_line
    .panel
      ul.panel_left
        img(src="../assets/img/LOGO.png" height=70 style="    filter: alpha(Opacity=50);opacity: 0.5; ")
        li.panel_left
          a FAQ
        li.panel_left
          a Контакты
        li.panel_left
          a Пользовательское соглашение
      .panel_right
        a tech_mail@mail.com
</template>

<script>
export default {
  components: {
  }
}
</script>

<style>
.panel{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
.panel ul{
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 19px; /* Отступ слева в браузере IE и Opera */
  padding-left: 0; /* Отступ слева в браузере Firefox, Safari, Chrome */
}
.panel li{
  list-style-type: none;
  margin-left: 47px;
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  color: #FFFFFF;
}
.panel_right{
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  text-align: right;
  color: #FFFFFF;
  margin-right: 55px;
}
.buts ul{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.header {
  height: 86px;
  background: radial-gradient(50% 50% at 50% 100%, rgba(88, 9, 199, 0.86) 0%, rgb(75, 3, 168) 100%);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
  position: relative;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.buts{
  display: flex;
  align-items: center;
  flex-direction: row;
  padding-left: 0;
  margin-left: 19px;
}

.buts li {
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex-direction: row;
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  color: #FFFFFF;
  padding: 17px;
}

.buts_text{
  margin: 0 6px;
}

.lk{
  display: flex;
  align-items: center;
  flex-direction: row;
  padding: 25px;
  padding-right:0px;
}
.lk_but{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 145px;
  height: 37px;
  background: #FFBC00;
  box-shadow: 0px 4px 4px #35007A;
  border-radius: 25px;
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  color: #000000;
  margin-right: 25px;
}
.user{
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  padding: 7px;
}
.user_info{
  display: flex;
  flex-direction: column;
  margin-left: 14px;
  font-family: Proxima Nova;
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  color: #FFFFFF;
  margin-right: 25px;
}

.footer{
  height: 86px;
  background: radial-gradient(50% 50% at 50% 100%, rgba(88, 9, 199, 0.86) 0%, rgb(75, 3, 168) 100%);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
  position: absolute;
  left: 0;
  bottom: 0;
  width: 100%;
  flex-direction: column;
}
.footer_line{
  position: relative;
  top:0;
  height: 7px;
  width: 100%;
  background: #FFBC00;
}

@font-face {
  font-family: "Proxima Nova";
  src: url("../assets/fonts/ProximaNova-Light.ttf") format("truetype");
  font-style: normal;
  font-weight: normal;
}
</style>

