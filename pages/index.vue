<template>
  <div :class="$style.main">
    <div :class="$style.box">
      <Header />
      <Slider />
      <Cards />
    </div>
  </div>
</template>
<script>
import Header from '@/components/header/Header.vue'
import Slider from '@/components/Slider/Slider.vue'
import Cards from '@/components/Cards/Cards.vue'
export default {
  components: {
    Header,
    Slider,
    Cards
  }
}
</script>
<style lang="scss" module>

.main{
  width: 100%;
  font-family: 'Righteous';
}
.box {
  max-width: 1235px;
  margin: 0 auto;
  padding-left: 10px;
  padding-right: 10px;

}

@media(max-width: 1215px){
.box{
    max-width: 1000px;

}
}

@media(max-width: 1000px){
.box{
    max-width: 800px;

}
}
@media(max-width: 800px){
.box{
    max-width: 600px;
}
}
</style>
