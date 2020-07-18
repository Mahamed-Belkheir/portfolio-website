<template>
    <div class="container">
        <div class="choosable" v-for="(value, i) in items" :key="value[0]"
            :class="{active: chosen == i}"
            v-on:click="pick(i)"
        >
            {{value[0]}}
        </div>
    </div>
</template>

<script>
export default {
    props: {
        items: Array,
        cb: Function
    },
    data: function() {
        return {
            chosen: 0
        }
    },
    methods: {
        pick(i) {
            this.chosen = i
            this.cb(i)
        }
    }
}
</script>

<style scoped>


.choosable {
    text-align: center;
    padding: 8px;
    font-weight: bold;
    border: 2px solid white;
   
}
.active {
    font-weight: bold;
    border: 2px solid;
    border-image-slice: 1;
    border-image-source: linear-gradient(
        to left,
        #2F80ED,
        #6FCF97
    );
    
}
</style>