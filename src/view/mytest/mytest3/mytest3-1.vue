<template>
  <div>
    mytest3-1
    <Button type="info" @click="jump(1)">Info</Button>
    <Button type="success" @click="jump(2)">Success</Button>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  methods: {
    jump (type) {
      if (type == '1') {
        this.$router.push('/mytest/mytest3/mytest3-1/mytest3info')
      } else {
        this.$router.push({ name: 'mytest3success' })
      }
    }
  }
}
</script>

<style lang="scss" scoped>
</style>
