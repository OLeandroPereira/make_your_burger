<template>
  <div class="message-container">
    <p>{{ msg }}</p>
  </div>
</template>

<script>
export default {
  name: "Message",
  props: {
    msg: String
  }
}
</script>

<style scoped>
  .message-container {
    color: #004085;
    background-color: #CCe5FF;
    border-radius: 2px solid #B8DAFF;
    padding: 10px;
    max-width: 400px;
    margin: 30px auto;
  }
</style>