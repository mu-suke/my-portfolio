<template>
  <v-container
    fill-height
    fluid
    class="mx-auto"
  >
    <div class="text-center py-4 mb-4">
      <v-btn color="white" large>
        <nuxt-link to="about">
          About
        </nuxt-link>
      </v-btn>
    </div>
    <div class="text-center py-4 mb-4">
      <v-btn color="white" large>
        <nuxt-link to="work">
          Work
        </nuxt-link>
      </v-btn>
    </div>
    <div class="text-center py-4 mb-4">
      <v-btn color="white" large>
        <nuxt-link to="contact">
          Contact
        </nuxt-link>
      </v-btn>
    </div>
  </v-container>
</template>

<script>

export default {
  transition: 'out-in'
}
</script>
