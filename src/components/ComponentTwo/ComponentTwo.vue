<template>
  <div id="ComponentTwo">
    <input placeholder="type colour" type="text" v-model="keyword" />
    <div class="box" v-bind:style="{backgroundColor: keyword}"></div>
  </div>
</template>

<script>
import './componentTwo.scss';

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
