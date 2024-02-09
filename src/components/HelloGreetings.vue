<template>
<h1>FRUITS ITEMS</h1><br>
<div class="container"  @click.prevent="countClicks">
    <div class="first">
        <h2> Apple </h2>
        <h3> I like Apples</h3>
        <p id="red">You have clicked me {{ count }} times.</p>
    </div><br>
    <div class="second">
        <h2> grapes </h2>
        <h3> I like Grapes</h3>
        <p id="red">You have clicked me {{ count }} times.</p>
    </div><br>
    <div class="third">
        <h2> Banana </h2>
        <h3> I like bananas</h3>
        <p id="red">You have clicked me {{ count }} times.</p>
    </div>
</div>
</template>

<script>
import { ref } from 'vue';
export default {
    setup() {
        let clicks = ref(0);

        function countClicks() {
            clicks = +1;
        }
        return {
            count: clicks,
            countClicks: countClicks
        }
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
.first,
.second,
.third {
    border: dashed black 1px;
    display: inline-block;
    margin: 10px;
    padding: 10px;
    background-color: lightgreen;

}

#red {
    font-size: medium;
    color: brown;
}
</style>
