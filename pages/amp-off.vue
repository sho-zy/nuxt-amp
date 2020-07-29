<template>
  <div>
    <h1>Not AMP Page</h1>
    <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
    <p>
      <img
        src="https://pbs.twimg.com/profile_images/1284697347545391104/-FlyD_jc_200x200.jpg"
        width="200"
        height="200"
      />
    </p>
    <p><nuxt-link to="/" v-text="'TOP'" /></p>
    <p><nuxt-link to="/amp-on" v-text="'アンプページ'" /></p>
    <p><nuxt-link to="/amp-off" v-text="'通常ページ'" /></p>
    <section id="idOne">
      <h2 v-text="'idOne'" />
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
    </section>
    <section id="idTwo">
      <h2 v-text="'idTwo'" />
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
    </section>
    <section id="idThree">
      <h2 v-text="'idThree'" />
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
    </section>
    <section id="idFour">
      <h2 v-text="'idFour'" />
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
      <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
    </section>
    <section class="api-contsiner">
      <h2 v-text="'topページからHTTP通信でデータ取得'" />
      <code>
        {{ posts }}
      </code>
    </section>
  </div>
</template>
<script>
export default {
  async asyncData({ $axios }) {
    const url = 'https://gifted-swirles-2a2b21.netlify.app'
    const response = await $axios.$get(url)
    return {
      posts: response,
    }
  },
}
</script>
