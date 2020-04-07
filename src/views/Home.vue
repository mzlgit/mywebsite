<template>
  <div class="home">
    <BaseHeader/>
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
