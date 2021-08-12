<template>
    <div id="app">
        <h1>Calculadora VueJS</h1>
        <Calculator />
    </div>
</template>

<script>
import Calculator from './main/Calculator'

export default {
    components: { Calculator }
}
</script>

<style>
@font-face {
    font-family: "RobotoMono";
    src: url("./fonts/RobotoMono-Thin.ttf");
}

* {
    font-family: "RobotoMono", monospace;
}

body {
    margin: 0;
}

#app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #fff;
    background: linear-gradient(to left,  #654ea3 10%, #eaafc8 100%);
}
</style>