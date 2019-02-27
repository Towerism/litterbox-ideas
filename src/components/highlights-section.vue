<template lang="pug">
  section#highlights.wrapper.style3
    .title The Endorsements
    .container
      .row.aln-center
        .col-4.col-12-medium(v-for="{ node } in $static.posts.edges")
          section.highlight
            g-link.image.featured(:to='node.path')
              g-image.fitted-image(:src='node.heroImage.file.url')
            h3
              g-link(:to='node.path') {{node.title}}
            p {{node.description}}
            ul.actions
              li
                g-link.button.style1(:to='node.path') Read More
</template>

<static-query>
query Posts {
  posts: allContentfulBlogPost {
    edges {
      node {
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
  }
}
</static-query>

<style lang="scss" scoped>
.fitted-image {
  object-fit: cover;
  max-height: 205px;
}
</style>
