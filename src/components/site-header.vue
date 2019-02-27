<template lang="pug">
  section#header.wrapper
    // Logo
    #logo
      h1
        a(href='index.html') Litterbox Ideas
      p Sometimes we get this best ideas in the litterbox
    // Nav
    nav#nav
      ul
        li.current
          g-link(to="/") Home
        li
          g-link(to="/blog-post") Food
        li
          g-link(to="/blog-post") Arts & Crafts
        li
          g-link(to="/blog-post") Random Musings
</template>
