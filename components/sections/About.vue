<template>
  <div class="section">
      <div class='item'>
        <Header title="About me"> </Header>
        <div class="text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer pulvinar mi venenatis neque malesuada, eu convallis felis rutrum. Quisque ullamcorper mauris sed tortor vulputate aliquam. Mauris vel feugiat ex.
        </div>
      </div>
      <div class='item side'>
        <Outlinebox class="box1"> </Outlinebox>
        <Outlinebox class="box2"> </Outlinebox>
        <Outlinebox class="box3"> </Outlinebox>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.item {
    width: 100%;
    height: 100%;
    size:100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.text {
    width: 65%;
    font-size: 24px;
}

.side {
    margin-top: 10vh;
}
.box1 {
    width: 28vh;    
    height: 28vh;
    margin-bottom: -33vh;
    margin-left: -8vh;
    transform: rotate(18deg);
}
.box2 {
    width: 33vh;    
    height: 33vh;
    transform: rotate(8deg);
}
.box3 {
    width: 23vh;    
    height: 23vh;
    transform: rotate(25deg);
    margin-top: -25vh;
    margin-left: -12vw;    
}
</style>