<template>
  <div>
    <section-title
      :icon="icon"
      :title="title"
    />
  </div>
</template>

<script>
import SectionTitle from '~/components/atoms/SectionTitle'

export default {
  components: {
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
