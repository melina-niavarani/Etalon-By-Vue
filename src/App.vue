<template>
  <body>
    <header>
      <NavItems/>
    </header>
    <router-view></router-view>
  </body>
</template>

<script>
import NavItems from '@/components/header/NavItems.vue'

export default {
  components: {
    NavItems,

  }
}

</script>

