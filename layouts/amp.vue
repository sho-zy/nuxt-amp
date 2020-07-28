<template>
  <amp-body>
    <amp-sidebar id="sidebar1" layout="nodisplay" side="right">
      <ul>
        <li class="red-text">Nav item 1</li>
        <li><a href="#idTwo" on="tap:idTwo.scrollTo">Nav item 2</a></li>
        <li>Nav item 3</li>
        <li><a href="#idFour" on="tap:idFour.scrollTo">Nav item 4</a></li>
        <li>Nav item 5</li>
        <li>Nav item 6</li>
      </ul>
    </amp-sidebar>
    <Nuxt />
  </amp-body>
</template>
<script>
export default {}
</script>
<style>
@import '~/assets/styles/default.amp.css';
</style>
