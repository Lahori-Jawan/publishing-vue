
<template>
    <Border>  <!-- Elborder component -->
        <div class="elborder">
            <p>The counter is set to <b>{{counter}}</b>.</p>
            <button @click="counter += 1">Click +1</button>
            <button @click="counter -= 1">Click -1</button>
            <button @click="counter = initCounter">Reset</button>
        </div>
    </Border>
</template>

<script>
// import Border from './DBug'
// import Border from '../dist/elborder.esm'
import Border from 'elborder';
export default {
    name: 'Elborder', // vue component name
    data() {
        return {
            counter: 5,
            initCounter: 5,
        };
    },
    components: {
        Border
    }
}
</script>

<style scoped>
    .elborder {
        display: block;
        width: 400px;
        margin: 25px auto;
        border: 1px solid #ccc;
        background: #eaeaea;
        text-align: center;
        padding: 25px;
    }
    .elborder p {
        margin: 0 0 1em;
    }
</style>
