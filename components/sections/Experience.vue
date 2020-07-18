<template>
  <div class="section">
      <div class="item">
          <Header title="Experience"></Header>
        <div class="text">{{text}}</div>
      </div>
      <div class="item">
          <Options :items="experiences" :cb="publish"> </Options>
      </div>
  </div>
</template>

<script>

export default {

    data: function() {
       return {
            experiences: [
            ["experience one", "Lorem one ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex."],
            ["experience two", "Lorem two ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex."],
            ["experience three", "Lorem three ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex."],
            ],
           
            text: ""
        }
    },
    methods: {
           publish(i) {
               this.text = this.experiences[i][1]
           }
    },
    mounted() {
        this.text = this.experiences[0][1]
    }
    

}
</script>

<style scoped>
.item {
    margin-top: -10vh;
    width: 100%;
    height: 100%;
    size:100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.items-list {
    display: flex;
    flex-direction: column;
}

.text {
    margin-left: 8vw;
}
</style>