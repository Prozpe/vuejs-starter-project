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
