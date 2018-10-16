<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <li v-for="review in reviews">{{ review.rating }} STARS - {{ review.reviewer }}: {{ review.text }}</li>
  </div>
</template>

<style>
</style>

<script>
export default {
  data: function() {
    return {
      message: "Hello world!",
      reviews: [
      	{ 
          text: "Vue.js is the best thing since sliced bread!",
          rating: 5,
          reviewer: "Burton Wax"
        },
        { 
          text: "I love Vue.js, especially when I'm programming!",
          rating: 4,
          reviewer: "Emily Post"
        },
        { 
          text: "Vue.js is waaaaay better than Chinese Checkers.",
          rating: 2,
          reviewer: "Angela Pearson"
        },
        { 
          text: "Vue.js so terrible, what am I doing?",
          rating: 1,
          reviewer: "Ace the Cat"
        }
      ]
    };
  },
  created: function() {},
  methods: {},
  computed: {}
};
</script>