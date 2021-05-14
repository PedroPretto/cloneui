<template>
  <div class="home">
    <Tweet v-for="tweet in tweets" :key="tweet._id" :tweetInfo="tweet" />
  </div>
</template>

<script>
import Tweet from "../components/Tweet";
import tweets from "../tweets";
export default {
  components: {
    Tweet,
  },
  setup() {
    return {
      tweets,
    };
  },
};
</script>
