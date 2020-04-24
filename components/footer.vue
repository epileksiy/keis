<template lang="pug">
  .footer
    .footer_line
    .panel
      ul
        img(src="../static/img/LOGO.png" height=70 style="    filter: alpha(Opacity=50);opacity: 0.5; ")
        li
          a FAQ
        li
          a Контакты
        li
          a Пользовательское соглашение
      .panel_right
        a tech_mail@mail.com
</template>

<script>
    export default {
        name: "footer"
    }
</script>

<style>
.footer{
  display: flex;
  justify-content: space-around;
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
.panel{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}
</style>
