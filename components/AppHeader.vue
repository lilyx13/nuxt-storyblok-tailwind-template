<script>
import { defineComponent, ref, computed } from '@vue/composition-api'
export default defineComponent({
  props: {
    info: {
      type: Object,
      default() {
        return { title: 'Standard Header' }
      }
    }
  },
  setup(props) {
    const capitalizedTitle = ref(props.info.title.toUpperCase())

    // Playing with names
    const firstName = ref('')
    const lastName = ref('')
    const fullName = computed(() => {
      return `${firstName} ${lastName}`
    })
    return {
      capitalizedTitle,
      fullName
    }
  }
})
</script>

<template>
  <header class="my-10 text-center">
    <h2>{{ capitalizedTitle }}</h2>
  </header>
</template>
