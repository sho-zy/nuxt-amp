<template>
  <amp-body>
    <amp-sidebar id="sidebar" layout="nodisplay" side="right">
      <ul>
        <li class="red-text">Nav item 1</li>
        <li><a href="#idTwo" on="tap:idTwo.scrollTo">Nav item 2</a></li>
        <li>Nav item 3</li>
        <li><a href="#idFour" on="tap:idFour.scrollTo">Nav item 4</a></li>
      </ul>
    </amp-sidebar>
    <button on="tap:sidebar.close">Close sidebar</button>
    <button on="tap:sidebar.toggle">Toggle sidebar</button>
    <Nuxt />
  </amp-body>
</template>
<script>
export default {}
</script>
<style>
@import '~/assets/styles/default.amp.css';
</style>
