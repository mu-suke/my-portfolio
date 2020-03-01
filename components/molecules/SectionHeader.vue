<template>
  <div>
    <section-divider />
    <section-title :icon="icon" :title="title" />
  </div>
</template>

<script>
import SectionDivider from '~/components/atoms/SectionDivider'
import SectionTitle from '~/components/atoms/SectionTitle'

export default {
  components: {
    SectionDivider,
    SectionTitle
  },
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
