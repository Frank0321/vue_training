<template>
  <div>
    <h2>{{header}}</h2>
    <input type="text" class="form-control" v-model="val" ref="child-input">
  </div>
</template>

<script>
export default {
  name: "demo-item",
  data() {
    return {
      header: '標題',
      val: '輸入框'
    }
  },
  methods: {
    focus() {
      this.$refs["child-input"].focus();
    },
    renameHeader(data){
      this.header = data;
    }
  }
}
</script>

<style scoped>

</style>