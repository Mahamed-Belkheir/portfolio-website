<template>
  <div class="section">
      <div class="item">
            <Header title="Projects"></Header>
            <div class="project_description">
                <div class="project_name">{{projects[pos][0]}}</div>
                <div class="text">{{projects[pos][1]}}</div>
                <a target="_blank" class="link" :href="projects[pos][2]">Github</a>
            </div> 
      </div>
      <div class="item">
          <Outlinebox class="box"> </Outlinebox>
          <Options :items="projects" :cb="publish"> </Options>
      </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            projects: [
                ["project one", "Lorem one ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex.",
                "https://github.com/Mahamed-Belkheir"],
                ["project two", "Lorem two ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex.",
                "https://github.com/Mahamed-Belkheir"],
                ["project three", "Lorem three ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex.",
                "https://github.com/Mahamed-Belkheir"],
            ],
            pos: 0
        }
    },
    methods: {
        publish(i) {
            this.pos = i
        }
    },
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

.project_description {
    margin-left: 8vw;
    border: 2px solid;
    padding: 20px;
    border-image-slice: 1;
    border-image-source: linear-gradient(
        to left,
        #2F80ED,
        #6FCF97
    );
    display: flex;
    flex-direction: column;
}

.project_name {
    font-size: 140%;
    padding-top: 10px;
    padding-bottom: 10px;;
}

.link {
    text-decoration: none;
    color: #2F80ED;
    padding-top: 10px;
    align-self: flex-end;
}


.box {
    width: 70vh;    
    height: 70vh;
    margin-bottom: -70vh;
    margin-right: -25vw;
    transform: rotate(6deg);
    z-index: -1;
}

</style>