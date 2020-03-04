<template>
  <main>
    <h4 class="caption">Зимбабве</h4>
    <Countries />
    <Request />
  </main>
</template>

<script>
import Countries from '@/components/Countries.vue'
import Request from '@/components/Request.vue'

export default {
  name: 'Main',
  components: {
    Countries,
    Request
  }
}
</script>