<template>
  <header>
    <h2>{{ capitalizedTitle }}</h2>
    <p>{{ description }}</p>
    <p>{{ fullName }}</p>
  </header>
</template>
<script>
import { defineComponent, ref, computed } from '@vue/composition-api'
export default defineComponent({
  props: {
    info: {
      type: Object,
      default() {
        return { name: 'Hello' }
      }
    }
  },
  setup(props) {
    const capitalizedTitle = ref(props.info.name.toUpperCase())
    const description = 'A bunch of stuff'
    const firstName = 'jane'
    const lastName = 'doe'
    const fullName = computed(() => {
      return `${firstName}${lastName}`
    })
    return {
      description,
      fullName,
      capitalizedTitle
    }
  }
})
</script>
