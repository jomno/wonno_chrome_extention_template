<template>
  <el-badge :value="12" class="item">
    <el-button size="small" @click="navigate('https://wantknow.tistory.com')">원노의 원트노로 이동</el-button>
  </el-badge>
</template>
<script>
  export default {
    data: () => ({
    }),
    computed: { },
    created () { },
    mounted () { },
    methods: {
      navigate (url) {
        chrome.tabs.create({ url: url })
      }
    }
  }
</script>
<style>
  .item {
    margin-top: 10px;
    margin-right: 40px;
  }
</style>
