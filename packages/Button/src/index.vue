<template>
  <button
    :class="[`x-button--${size}`, { 'is-plain': plain },`x-button--${type}`,{'is-round':round}]"
    @click="handleClick"
    class="x-button"
    
  >
    <span> <slot></slot> </span>
  </button>
</template>
<script>
export default {
  name: "x-button",
  props: {
    size: {
      type: String
    },
    type: {
      type: String,
      default: "default"
    },
    round: {
      type: Boolean,
      default: false
    },
    plain: {
      type: Boolean,
      default: false
    }
  },
  methods: {
    handleClick(e) {
      this.$emit("click",e);
    }
  }
};
</script>
<style scoped lang="less">
@import url("./css.less");
</style>
