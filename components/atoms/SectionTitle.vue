<template>
  <h2 class="display-1 text-center">
    <v-icon class="pb-2" size="48">
      mdi-{{ icon }}
    </v-icon>
    {{ title }}
  </h2>
</template>

<script>
export default {
  props: {
    icon: {
      type: String,
      required: true,
      default: ''
    },
    title: {
      type: String,
      required: true,
      default: ''
    }
  }
}
</script>
