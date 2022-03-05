<script>
export default {
  name: 'IndexPage',
  setup() {
    const test = 'Test Text'
    return { test }
  }
}
</script>

<template>
  <div>
    <p>{{ test }}</p>
  </div>
</template>
