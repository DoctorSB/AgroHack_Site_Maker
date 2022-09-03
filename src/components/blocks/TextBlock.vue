<template>
  <div class="stndr-block"
       :id = "id"
       :draggable="draggable"
       @dragstart="dragStart"
       @dragover.stop
  >
    <slot/>
    <p>your text</p>
  </div>
</template>

<script>
export default {
  props:["id", "draggable"],
  methods:{
    dragStart: e => {
      const target = e.target;
      e.dataTransfer.setData('card_id', target.id);

      setTimeout(() => {
          target.style.display = "none"
          },0);
}
  }

}
</script>

<style scoped>
.txt-block{
  height: 150px;
  width: 85%;
  background: turquoise;

}
</style>