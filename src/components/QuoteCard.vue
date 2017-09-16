<template>
    <div id="quote-card">
        <p>{{ quote }}</p>
    </div>
</template>

<script>
    export default {
        props: ['quote']
    }
</script>

<style scoped lang="scss">
    div {
        border: 1px solid #251d1d;
        border-radius: 10px;
        padding: 10px;
        margin: 10px 10px 0 0;
        display: inline-block;
    }
    p {
        font-style: italic;
    }
</style>
