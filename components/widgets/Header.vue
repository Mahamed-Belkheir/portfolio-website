<template>
  <div class="header">
      <div class="text">{{title}}</div>
  </div>
</template>

<script>
export default {
    props: {
        title: String
    }
}
</script>

<style scoped>

.text {
    font-size: 36px;
}

.header {
    display: flex;
    border-bottom: 2px solid;
    border-image-slice: 1;
    border-image-source: linear-gradient(
    to left,
    #2F80ED,
    #6FCF97
    );
    width: 100%;
    margin-bottom: 5vw;
    margin-left: 10vw;
}
</style>