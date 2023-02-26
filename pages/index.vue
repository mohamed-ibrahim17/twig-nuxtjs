<template>
  <div style="margin: 2rem; text-align: center">
    <NuxtLogo />

    <TwigRenderer
      template-path='templates/posts.twig'
      :options="templateOptions"
    />
  </div>
</template>

<script>
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  data() {
    return {
      templateOptions: {
        posts: [
          {
            title: 'Header 1',
            body: 'Body 1'
          },
          {
            title: 'Header 2',
            body: 'Body 2'
          },
          {
            title: 'Header 3',
            body: 'Body 3'
          }
        ],

        name: 'Mohamed'
      }
    }
  },
})
</script>
