<template>
    <div class='section'>
        <div class="landing-text">
        <Outlinebox class="box3">
        </Outlinebox>
        <div class="text-box">
                <h2>Hello, I'm Mahamed,<br>
                    a Software Developer <br>
                </h2>
                 <div class="small-text"><small>who likes to code.</small></div>
                 <div class="action-btn"> Get to know me</div>
        </div>
        </div>
        <div class="boxes">
            <Fullbox class="box2"> </Fullbox>
            <Outlinebox class="box1"> </Outlinebox>
        </div>
    </div>
</template>

<script>

export default {

}
</script>

<style scoped>

.boxes {
    width: 100%;
    height: 100%;
    size:100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.box1 {
    width: 30vh;
    height: 30vh;
    transform: rotate(35deg);
    margin-left: 3vw;
    margin-top: 5vh;
}

.box2 {
    width: 30vh;
    height: 30vh;
    transform: rotate(-35deg);
    margin-right: -10vw;
    margin-top: -15vh;
}

.landing-text {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.box3 {
    width: 70vh;
    height: 70vh;
    transform: rotate(35deg);
    margin-left: -15vw;
    margin-top: 10vh;
}

.text-box {
    margin-left: -35vw;
    font-size: 170%;
}

.small-text {
    margin-top: -5vh;
}

.action-btn {
    background-color: #2DACDB;
    border-radius: 6px;
    color: white;
    text-align: center;
    width: 50%;
    margin-top: 25px;
    padding: 10px;
}

</style>