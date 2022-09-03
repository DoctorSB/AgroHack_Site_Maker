<template>
  <div class="r-side">
    <p>Доступные Элементы </p>
    <div class="r-side-column">
      <text-block
          :id="id"
          @dragover.prevent
          @drop.prevent="drop"
      >
      </text-block>
      <slider-block/>
      <text-block/>
    </div>
  </div>
</template>

<script>
import TextBlock from "@/components/blocks/TextBlock";
import SliderBlock from "@/components/blocks/SliderBlock";


export default {
  components: {
    TextBlock, SliderBlock
  },
  props: ["id"],
  methods: {
    drop: e=>{
      const card_id = e.dataTransfer.getData('card_id')
      const card = document.dataTransfer.getData(card_id)
      card.style.display = "block"
      e.target.appendChild(card)
    }
  }
}
</script>

<style scoped>
.r-side{
  overflow-y:auto;
  width: 15%;
  background: blueviolet;
  display: flex;
  flex-direction: column;
}
</style>