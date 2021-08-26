<template>
  <view>
    <button title="Botón arriba"></button>
    <scroll-view :horizontal="true" :style="{ backgroundColor: 'blue' }">
      <button title="Botón arriba"></button>
      <text :style="{ padding: 40 }"> Hola 1 </text>

      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> Hola 1 </text>
      <text :style="{ padding: 40 }"> ************* </text>
    </scroll-view>
    <scroll-view :style="{ backgroundColor: 'red', height: 300 }">
      <text v-for="i in a" v-bind:key="i" :style="{ padding: 40 }"> Hola {{ i }} </text>
    </scroll-view>
    <button title="Botón arriba"></button>
  </view>
</template>

<script>
export default {
  data() {
    return {
      a:[1,2,3,4,5,6,7,8,9,10,11,12,13,14,15]
    }
  },
}
</script>