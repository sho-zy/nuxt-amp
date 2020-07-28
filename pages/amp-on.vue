<template>
  <div>
    <h1>AMP Page</h1>
    <p>てすとてすとてすとてすとてすとてすとてすとてすとてすとてすと</p>
    <p>
      <img
        src="https://pbs.twimg.com/profile_images/1284697347545391104/-FlyD_jc_200x200.jpg"
      />
    </p>
    <p><nuxt-link to="/" v-text="'TOP'" /></p>
    <p><nuxt-link to="/amp-on" v-text="'アンプあり(通常)'" /></p>
    <p><nuxt-link to="/amp/amp-on" v-text="'アンプあり(AMP)'" /></p>
    <p><nuxt-link to="/amp-off" v-text="'アンプなし(通常)'" /></p>
    <p><nuxt-link to="/amp/amp-off" v-text="'アンプなし(AMP)'" /></p>
  </div>
</template>
