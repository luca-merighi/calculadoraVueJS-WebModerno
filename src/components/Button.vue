<template>
  <button 
    class="button" 
    :class="{double, triple, operation}" 
    @click="$emit('onClick', label)" >
      {{label}}
  </button>
</template>

<script>
export default {
    props: {
        label: {},
        operation: { type: Boolean},
        double: { type: Boolean},
        triple: { type: Boolean}
    }
}
</script>

<style>
:root {
    --bg-button: #8a41b1;
    --border-button: 1px solid #ff8fc7;
}

.button {
    font-size: 1.4em;
    background-color: var(--bg-button);
    border: none;
    border-right: var(--border-button);
    border-bottom: var(--border-button);
    outline: none;
    color: #fff;

}

.button:active {
    background-color: #9b0794;
}

.button.double {
    grid-column: span 2;
}

.button.triple {
    grid-column: span 3;
}

.button.operation {
    background-color: #8a079b;
    color: #fff;
}

.button.operation:active {
    background-color: #b61bcacc;
}


</style>