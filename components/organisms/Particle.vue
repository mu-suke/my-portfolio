<template>
  <div id="snowfall">
    <vue-typer
      :text="['Arya Stark','Jon Snow','Daenerys Targaryen','Melisandre','Tyrion Lannister']"
      :repeat='Infinity'
      :shuffle='false'
      initial-action='typing'
      :pre-type-delay='70'
      :type-delay='70'
      :pre-erase-delay='2000'
      :erase-delay='250'
      erase-style='select-all'
      :erase-on-complete='false'
      caret-animation='blink'
    ></vue-typer>
  </div>
</template>

<script>
import { VueTyper } from 'vue-typer'
import snow from '~/assets/js/particles/snow.js'

export default {
  components: {
    VueTyper
  },
  mounted () {
    // 画面が表示された時にparticles.jsを動かす
    window.particlesJS('snowfall', snow.data)
  }
}
</script>

<style>
#snowfall {
  background-color: #333333;
  width: 100%;
  height: 100vh;
  z-index: 0;
}
</style>
