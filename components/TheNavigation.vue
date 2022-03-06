<template>
  <nav class="mx-4 h-8">
    <ul class="flex items-baseline flex-wrap gap-4">
      <li v-for="link in navLinks" :key="link.id">
        <nuxt-link :to="link.url" class="flex gap-2">
          ><span>{{ link.text }}</span>
        </nuxt-link>
      </li>
    </ul>
  </nav>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
  setup() {
    const navLinks = [
      {
        text: 'About',
        url: 'about'
      },
      {
        text: 'Blog',
        url: 'blog'
      },
      {
        text: 'Contact',
        url: 'contact'
      }
    ]
    return {
      navLinks
    }
  }
})
</script>
