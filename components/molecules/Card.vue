<template>
  <v-card class="card">
    <nuxt-link v-bind:to="{ name: 'blog-slug', params: { slug: slug }}" class="wrapper">
      <v-container>
        <v-row>
          <v-col cols="4">
            <v-img
              class="card_image"
              :src="headerImage.fields.file.url"
              height="200"
              width="200"
              contain
            >
            </v-img>
          </v-col>
          <v-col cols="8">
            <h3 class="card_title">{{ title }}</h3>
            <p class="card_date">{{ (new Date(publishedAt)).toLocaleDateString() }}</p>
          </v-col>
        </v-row>
      </v-container>
    </nuxt-link>
  </v-card>
</template>

<script>
export default {
  props: ['title', 'slug', 'headerImage', 'publishedAt']
}
</script>

<style scoped>
.card {
  box-shadow: 1px 2px 3px 1px rgba(0,0,0,0.2);
  border: 0.5px solid rgb(57, 72, 85);
  padding: 10px 20px;
  margin: 10px 10px;
  text-align: center;
  z-index: 10;
}
.wrapper {
  text-decoration: none;
}
.card_title {
  font-size: 1.2rem;
}
.card_date {
  font-size: 0.7rem;
  color: rgb(57, 72, 85);
  text-align: right;
}
.card_image {
  max-height: 100px;
}
</style>