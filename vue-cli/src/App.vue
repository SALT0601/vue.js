<template>
  <div><AppHeader v-bind:propsdata="str" v-on:renew="renewStr" /></div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
export default {
  data: function () {
    return {
      str: "Header",
    };
  },
  components: {
    AppHeader,
  },
  methods: {
    renewStr: function () {
      this.str = "hihi";
    },
  },
};
</script>

<style></style>
