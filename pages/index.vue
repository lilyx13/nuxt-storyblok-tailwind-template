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
    <h1>This is a Title</h1>
    <p>{{ test }}</p>
  </div>
</template>
