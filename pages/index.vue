<template lang="pug">
div
  div(class="header")
    div.nav
      div(class="buts")
        img(src="../assets/img/LOGO.png" height=70)
        div.buts.item
          img(src="../assets/img/Header/Vector.png" width=32 height=32)
          a.buts.item.text Апгрейд
        div.buts.item
          img(src="../assets/img/Header/Top.png" width=32 height=32)
          a.buts.item.text Битва за скин
        div.buts.item
          img(src="../assets/img/Header/Items.png" width=32 height=32)
          a.buts.item.text Предметы
        div.buts.item
          img(src="../assets/img/Header/Games.png" width=32 height=32)
          a.buts.item.text Игры
      div(class="lk")
        div.lk.user
          img(src="../assets/img/Header/Ава.png" height=58 width=57)
          div.lk.user.info
            a(style="font-weight:300;") Aska.again
            a(style="font-weight:600;") 276.76 ₽
        div.lk.yelbut
          a + Пополнить
        img(src="../assets/img/Header/exit.png" width=27 height=27 style="margin-right: 25px;")
  div.footer
    div.footer.line
    div.panel
      div.panel.leftside
        img(src="../assets/img/LOGO.png" height=70 style="    filter: alpha(Opacity=50);opacity: 0.5; ")
        div.panel.leftside.item
          a FAQ
        div.panel.leftside.item
          a Контакты
        div.panel.leftside.item
          a Пользовательское соглашение
      div.panel.rightside
          a tech_mail@mail.com
</template>

<script>
export default {
  components: {
  }
}
</script>

<style>
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
.footer .line{
  position: relative;
  top:0;
  height: 7px;
  width: 100%;
  background: #FFBC00;
}
.panel{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
.panel .leftside{
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-direction: row;
  margin-left: 20px;
  font: 14px/16px arial, helvetica, sans-serif;
  font-style: normal;
  font-weight: 600;
  color: #FFFFFF;
  padding: 6px;
}
.panel .leftside .item{
  display: flex;
  margin-left: 47px;
}
.panel .rightside{
  font: 14px/16px arial, helvetica, sans-serif;
  font-style: normal;
  font-weight: 600;
  color: #FFFFFF;
  padding: 6px;
  margin-right: 55px;
}
.nav{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.lk{
  display: flex;
  align-items: center;
  flex-direction: row;
}
.lk .yelbut{
  display: flex;
  justify-content: center;
  align-items: center;
  width: 145px;
  height: 37px;
  background: #FFBC00;
  box-shadow: 0px 4px 4px #35007A;
  border-radius: 25px;
  font: 14px/16px arial, helvetica, sans-serif;
  font-style: normal;
  font-weight: 600;
  color: #000000;
  margin-right: 25px;
}
.lk .user{
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
}
.lk .user .info{
  flex-direction: column;
  margin-left: 14px;
  font: 14px/16px arial, helvetica, sans-serif;
  font-style: normal;
  color: #FFFFFF;
  padding: 6px;
  margin-right: 25px;
}
.header {
  height: 86px;
  background: radial-gradient(50% 50% at 50% 100%, rgba(88, 9, 199, 0.86) 0%, rgb(75, 3, 168) 100%);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
  position: relative;
}

.buts{
  display: flex;
  align-items: center;
  justify-content: flex-start;
  flex-direction: row;
  margin-left: 20px;
}
.buts .item {
  display: flex;
  align-items: center;
  justify-content: space-around;
  flex-direction: row;
  font: 14px/16px arial, helvetica, sans-serif;
  font-style: normal;
  font-weight: 600;
  color: #FFFFFF;
  padding: 6px;
}
.buts .item .text{
  margin: 0 6px;
}
</style>

