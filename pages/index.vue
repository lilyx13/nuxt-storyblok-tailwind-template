<script>
export default {
  name: 'IndexPage',
  setup() {
    const pageInfo = { name: 'Home', description: 'This is the Home Page' }
    return { pageInfo }
  }
}
</script>

<template>
  <div>
    <AppHeader />
  </div>
</template>
