<template>
  <div class="home">
    <base-header/>
  </div>
</template>

<script>
// @ is an alias to /src
import BaseHeader from '@/components/BaseHeader.vue'

export default {
  name: 'Home',
  components: {
    BaseHeader
  }
}
</script>
