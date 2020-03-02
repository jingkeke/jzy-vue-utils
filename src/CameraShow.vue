<template>
  <span ref='countup'></span>
</template>

<script>
import { CountUp } from 'countup.js';

export default {
  name: 'CountTo',
  props:{
      endVal:{
        type:Number,
        required:true,
      },
      options:{
        type:Object,
        required:false
      }
  },
  data () {
    return {
      numAnim:null
    }
  },
  mounted(){
    this.initCountUp()
  },
  methods:{
    initCountUp(){
      this.numAnim = new CountUp(this.$refs.countup,this.endVal ,this.options)
      this.numAnim.start();
    }
  }
}
</script>

<style lang="scss">
</style>
