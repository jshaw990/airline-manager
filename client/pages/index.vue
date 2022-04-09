<template>
<div>
  {{ greeting }}
</div>
</template>

<script>
import { reactive, toRefs } from '@vue/composition-api'

export default {
  name: 'IndexPage',
  setup () {
    const state = reactive({
      greeting: 'Hello'
    })

    return {
      ...toRefs(state)
    }
  }
}
</script>
