<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <li v-for="review in reviews">{{ review.rating }} STARS - {{ review.reviewer }}: {{ review.text }}</li>
    <input v-model="reviews[2].text">

    <h3>Leave a review:</h3>
    Review: <input v-model="newReview.text">
    Rating: <input v-model="newReview.rating">
    Your Name: <input v-model="newReview.reviewer">
    <button v-on:click="addReview()">Add Review</button>

    <p>{{ newReview }}</p>

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
        }
      ],
      newReview: {text: "", rating: "", reviewer: ""}
    };
  },
  created: function() {},
  methods: {
  	addReview: function() {
  		this.reviews.push(this.newReview);
  	}
  },
  computed: {}
};
</script>


















