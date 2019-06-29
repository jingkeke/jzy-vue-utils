<template>
  <div id="app">
    <CountTo end-val="100"   ></CountTo>
  </div>
</template>

<script>
import CountTo from './CountTo'
export default {
  name: 'app',
  components:{CountTo},
  data () {
    return {

    }
  }
}
</script>

<style lang="scss">
</style>
