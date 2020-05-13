<template lang="pug">
  .header
    ul.buts
      img(src="../static/img/LOGO.png" height=70)
      li.buts
        a.buts_text Апгрейд
      li.buts
        a.buts_text Битва за скин
      li.buts
        a.buts_text Предметы
      li.buts
        a.buts_text Игры
    .topright
      .user
        .user_img
          img(src="../static/img/Header/picture.png" height=46 width=46)
        .user_info
          a(style="font-weight:300;margin-bottom:3px;") Aska.again
          a(style="font-weight:600;") 276.76 ₽
      .topright_but
        a + Пополнить
      img(src="../static/img/Header/exit.png" width=27 height=27 style="margin-right: 31.5px;")
</template>

<script>
    export default {
        name: "header.vue",
        methods: {
            ChangeImage: function(id,image){
                    var el=document.getElementById(id);
                    el.src=image;
            }
        }
    }
</script>

<style>
.user_img{
  height:58px;
  width: 58px;
  background: url("../static/img/Header/picture-border.png");
  background-size: contain;
  text-align: center;
  vertical-align: middle;
}
.user_img img{
  margin-top: 6px;
}
.panel ul{
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-left: 34px; /* Отступ слева в браузере IE и Opera */
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
.buts li :before{
  content: url("../static/img/Header/Top.png");
  display: inline;
  vertical-align: middle;
  align-items: center;
  margin-right: 10px;
}
.buts li:hover{
  background: radial-gradient(50% 50% at 50% 100%, rgba(120, 20, 199, 0.7) 0%, rgba(75, 3, 168, 0.8) 100%);
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
}
.buts ul{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding-left: 34px;
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
  margin-left: 34px;
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
  height: 100%;
}

.buts_text{
  margin: 0 6px;
}
.topright{
  display: flex;
  align-items: center;
  flex-direction: row;
  padding: 25px;
  padding-right:0px;
}
.topright_but{
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
</style>
