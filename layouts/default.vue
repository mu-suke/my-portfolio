<template>
  <v-app>
    <v-container
      fill-height
      fluid
      class="bg"
    >
      <transition mode="out-in">
        <nuxt class="mx-auto" />
      </transition>
    </v-container>
  </v-app>
</template>

<style>
html {
  font-family: "Source Sans Pro", 游ゴシック体, 'Yu Gothic', YuGothic, 'ヒラギノ角ゴシック Pro', 'Hiragino Kaku Gothic Pro', メイリオ, Meiryo, sans-serif;
  font-size: 16px;
}
h1, h2, h3 {
  font-weight: normal;
}
.title {
  color: #35495e;
  margin: 100px 0 30px;
  text-align: center;
}
.v-enter-active, .v-leave-active {
  transition: opacity 1s;
}
.v-enter, .v-leave-to {
  opacity: 0;
}
.bg {
  background-image: url("~@/assets/bg.jpg");
  background-position: center;
  background-size: cover;
  position: relative;
  z-index: 0;
  overflow: hidden;
}
.bg:before{
  content: '';
  background: inherit;
  -webkit-filter: blur(5px);
  -moz-filter: blur(5px);
  -o-filter: blur(5px);
  -ms-filter: blur(5px);
  filter: blur(5px);
  position: absolute;
  top: -5px;
  left: -5px;
  right: -5px;
  bottom: -5px;
  z-index: -1;
}
</style>
