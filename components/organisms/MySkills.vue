<template>
  <section class="skills">
    <section-header icon="file-document-edit-outline" title="Skills" />
    <v-row class="text-center" no-gutters>
      <v-col
        v-for="(skill, index) in skillList"
        :key="index"
        cols="4"
        xs="2"
      >
        <v-chip
          class="ma-2"
        >
          {{ skill }}
        </v-chip>
      </v-col>
    </v-row>
  </section>
</template>

<script>
import SectionHeader from '~/components/molecules/SectionHeader'

export default {
  components: {
    SectionHeader
  },
  data () {
    return {
      skillList: ['JavaScript(ES6)', 'Vue/Nuxt', 'Flutter', 'Python', 'Google App Script', 'C/C++', 'Firebase']
    }
  }
}
</script>
