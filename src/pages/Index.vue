<template lang="pug">
  Layout
    intro-section
    details-section
    highlights-section
</template>
<script>
import IntroSection from '~/components/intro-section'
import DetailsSection from '~/components/details-section'
import HighlightsSection from '~/components/highlights-section'

export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    IntroSection,
    DetailsSection,
    HighlightsSection
  }
}
</script>
