<template>
  <header>
    <div class="center-page">
      <div class="header-logo">
        <img src="" alt="">
      </div>
      <div class="header-bottoms">
        <ul>
          <li><a href="#">Компания</a></li>
          <li><a href="#">Каталог</a></li>
          <li><a href="#">Контакты</a></li>
        </ul>
      </div>
      <div class="header-end">
        <img src="">
        <img src="">
      </div>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style scoped>
a{
  text-decoration: none;
  color: aliceblue;
}
.center-page{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}
header{
  margin: 1% 12.5%;
  background-color: #222222;
  height: 64px;
}
.header-logo{
  height: 64px;
  width: 10%;
}
.header-bottoms{
  width: 80%;
  text-decoration: none;
}
li, ul{
  list-style: none;
  display: inline-block;
}
.header-end{
  width: 10%;
}
</style>