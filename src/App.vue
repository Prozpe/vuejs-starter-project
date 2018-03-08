<template>
  <div>
    <ComponentOne />
    <ComponentTwo />
    <Fetch />
  </div>
</template>

<script>
import ComponentOne from './components/ComponentOne/ComponentOne';
import ComponentTwo from './components/ComponentTwo/ComponentTwo';
import Fetch from './components/Fetch/Fetch';

export default {
  name: 'app',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      keyword: '',
      onOff: true,
    };
  },
  components: {
    ComponentOne,
    ComponentTwo,
    Fetch,
  },
};
</script>

<style lang="scss">
#app {
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
