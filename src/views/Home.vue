<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <h2>{{ secondMessage }}</h2>
  </div>
</template>

<style>
</style>

<script>
export default {
  data: function() {
    return {
      message: "Hello world!",
      secondMessage: "This is my second message"
    };
  },
  created: function() {},
  methods: {},
  computed: {}
};
</script>