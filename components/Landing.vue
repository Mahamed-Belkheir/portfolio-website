<template>
    <div class='landing'>
        <div class="boxes">
            <Outlinebox class="box1"> </Outlinebox>
            <Outlinebox class="box1"> </Outlinebox>
        </div>
    </div>
</template>

<script>

export default {

}
</script>

<style scoped>
.landing {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
    width: 100vw;
    height: 100vh;
}
.boxes {
    height: 25vh;
    grid-row: 3;
    grid-column: 4;
}

.box1 {
    width: 30vh;
    height: 30vh;
    transform: rotate(35deg);
}
</style>