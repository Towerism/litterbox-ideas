<template lang="pug">
  .layout
    #page-wrapper
      site-header
      slot
      site-footer
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<script>
import SiteHeader from '~/components/site-header'
import SiteFooter from '~/components/site-footer'

export default {
  components: {
    SiteHeader,
    SiteFooter
  }
}
</script>
