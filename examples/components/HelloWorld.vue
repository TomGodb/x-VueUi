<template>
  <div class="hello">
    <x-button type="danger"  :round="true" size="mini"  @click="asas" 
      >button</x-button
    >
  </div>
</template>
<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  methods: {
    asas() {
      console.log("22");
    }
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
