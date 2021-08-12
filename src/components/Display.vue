<template>
    <div class="display">
        {{value}}
    </div>
</template>

<script>
export default {
    props: ['value']
}
</script>

<style>
    .display {
        grid-column: span 4;
        background: #9e14b6;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        padding: 20px;
        font-size: 2.1em;
        overflow: hidden;

    }
</style>