<template>
  <div class="pc-x-list" element-path="pc/x-list">
  {{viewModel}}
  </div>
</template>

<script>
  export default {
    name: 'x-list',
    props: {
      elementData: {}
    },
    data () {
      return {
        viewModel: ''
      }
    },
    mounted () {
      this.init()
    },
    methods: {
      async init () {
        if (this.elementData !== undefined) {
          this.viewModel = this.elementData
        }
      }
    }
  }
</script>

<style lang="less">
  @import '~_style/index.less';
  .pc-x-list {
  	font-size: @font-size-base;
  }
</style>
