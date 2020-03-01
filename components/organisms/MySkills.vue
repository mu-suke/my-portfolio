<template>
  <section class="skills">
    <section-header icon="file-document-edit-outline" title="Skills" />
    <div class="text-center">
      <v-chip
        v-for="(skill, index) in skillList"
        :key="index"
        class="ma-2"
      >
        {{ skill }}
      </v-chip>
    </div>
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
