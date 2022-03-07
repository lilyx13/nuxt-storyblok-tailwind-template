<script>
export default {
  name: 'IndexPage',
  setup() {
    const pageInfo = {
      title: 'Home Page'
    }
    return { pageInfo }
  }
}
</script>

<template>
  <div class="flex flex-col justify-center items-center">
    <AppHeader :info="pageInfo" />
    <main clas="container mx-auto">
      <p class="max-w-prose">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Odit nesciunt
        nemo dolores dolore expedita quas assumenda officia culpa autem fugiat
        aspernatur ipsa suscipit dignissimos, reprehenderit iure, accusamus
        ipsam harum totam facere minus maiores nostrum pariatur atque! Iusto
        magnam ut maiores doloribus temporibus? Ipsam optio cum ab maiores
        tempore laudantium illum.
      </p>
    </main>
  </div>
</template>
