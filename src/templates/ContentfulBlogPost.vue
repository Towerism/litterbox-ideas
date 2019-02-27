<template lang="pug">
  Layout
    #main.wrapper.style2
      .title {{$page.post.title}}
      .container
        // Content
        #content
          article.box.post
            a.image.featured(href='#')
              g-image(:src='$page.post.heroImage.file.url')
            vue-markdown(:source="$page.post.body")
    highlights-section
</template>

<page-query>
query Post ($path: String!) {
  post: contentfulBlogPost (path: $path) {
    publishDate,
    title,
    path,
    heroImage {
      file {
        url
      }
    },
    description,
    body,
    author {
      name,
      shortBio
    }
  }
}
</page-query>

<script>
import HighlightsSection from '~/components/highlights-section'
import VueMarkdown from 'vue-markdown'

export default {
  components: {
    HighlightsSection,
    VueMarkdown
  }
}
</script>
