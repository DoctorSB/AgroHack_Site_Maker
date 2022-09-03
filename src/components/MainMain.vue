<template>
  <div class="main">
    <div class="center-page">
        <left-element/>
        <main-center/>
        <right-element/>
    </div>
  </div>
</template>

<script>
import RightElement from "@/components/RightElement";
import LeftElement from "@/components/LeftElement";
import MainCenter from "@/components/MainCenter";
export default {
  components: {
    RightElement, LeftElement, MainCenter
  },


}
</script>

<style scoped>
.main{
  display: flex;
  height: 560px;
  margin: 1% 1%;
}

.center-page{
  display: flex;
  width: 100%;
}
</style>