<template>
  <div>
      <img :src="tweet.img" :alt="tweet.handle + 'profile pricture'">
      <h5>Name: {{ tweet.name }}</h5>
      <h6>Handle: {{ tweet.handle }}</h6>
      <p>{{ tweet.tweet }}</p>
      <p>Likes: {{ tweet.likes }}</p>
  </div>
</template>

<script>
export default {
    name: 'tweet-list-item',
    props: ['tweet']
}
</script>

<style>
img {
    width: 100px;
    height: auto;
}
</style>