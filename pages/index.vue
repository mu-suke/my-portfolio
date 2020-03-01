<template>
  <v-container
    fluid
    class="pa-0"
  >
    <v-parallax
      dark
      src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
    >
      <v-row
        align="center"
        justify="center"
      >
        <v-col class="text-center" cols="12">
          <h1 class="display-1 font-weight-thin mb-4">
            Welcome to mu-suke's Portfolio Site!
          </h1>
          <h4 class="subheading">
            Ha Ha Ha!
          </h4>
        </v-col>
      </v-row>
    </v-parallax>
    <v-col
      xs="8"
      sm="8"
      lg="8"
      class="mx-auto"
    >
      <my-profile />
      <my-skills />
    </v-col>
  </v-container>
</template>

<script>
import MyProfile from '~/components/organisms/MyProfile.vue'
import MySkills from '~/components/organisms/MySkills'

export default {
  transition: 'slide-left',
  components: {
    MyProfile,
    MySkills
  }
}
</script>
