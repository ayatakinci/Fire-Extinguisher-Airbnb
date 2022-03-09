<template>
<div>
  <Hero-page />
  <LargeCard-display v-for="cardInfo in largeCardInfo"
  :key="cardInfo.id"
  :cardsSection="cardInfo" />
  </div>
</template>

<script>
import {largeCardSections} from "~/assets/data.js"
export default {
 data(){
   return{
     largeCardInfo: largeCardSections
   }
 }
}
</script>
