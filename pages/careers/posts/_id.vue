<template>
  <v-card
          class="mx-auto"
          max-width="344"
          outlined
  >
    <v-list-item three-line>
      <v-list-item-content>
        <div class="overline mb-4"> OVERLINE</div>
        <v-list-item-title class="headline mb-1">{{ item.title }}</v-list-item-title>
        <v-list-item-subtitle v-html="$md.render(item.body)"></v-list-item-subtitle>
      </v-list-item-content>
    </v-list-item>
  </v-card>
</template>

<script>
import axios from 'axios'

export default {
  async asyncData ({ params }) {
    const { data } = await axios.get(
      `https://yasutomog.microcms.io/api/v1/posts/${params.id}`,
      {
        headers: { 'X-API-KEY': process.env.API_KEY }
      }
    )
    return {
      item: data
    }
  }
}
</script>
