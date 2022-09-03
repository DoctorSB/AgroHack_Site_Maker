<template>
  <div class="app">
    <main-head/>
    <main-main/>
    <main-footer/>
  </div>
</template>

<script>
//import PostForms from "@/components/PostForms";
//import PostList from "@/components/PostList";
import MainHead from "@/components/MainHead";
import MainFooter from "@/components/MainFooter";
import MainMain from "@/components/MainMain";
export default {
  components: {
    MainHead, MainFooter, MainMain,
  },

}

</script>

<style>
*{
  font-family: Arial;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app{
  color: aliceblue;
  background-image: url("/img/back.jpg") ;
  background-repeat: no-repeat;
  background-size: 100%;
  display: flex;
  flex-direction: column;
  padding: 15px;
}
.stndr-block{
  -webkit-user-select: auto;
  -webkit-user-drag: auto;
  height: 150px;
  width: 85%;
  background: turquoise;
  border-radius: 8px;
  border: 2px solid bisque;
  cursor: initial;
}

</style>