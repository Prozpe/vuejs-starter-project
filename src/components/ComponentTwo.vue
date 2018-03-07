<template>
  <div id="ComponentTwo">
    <input placeholder="type colour" type="text" v-model="keyword" />
    <div class="box" v-bind:style="{backgroundColor: keyword}"></div>
  </div>
</template>

<script>
export default {
  name: 'ComponentTwo',
  data() {
    return {
      keyword: '',
      onOff: true,
    };
  },
  methods: {
    toggleOnOff() {
      this.onOff = !this.onOff;
    },
  },
};
</script>

<style lang="scss">
#ComponentTwo {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

.box {
  width: 100px;
  height: 100px;
  border: 1px solid rgba(0, 0, 0, 0.12);
  margin: 10px auto 0;
}
</style>
