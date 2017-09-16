<template>
    <div id="app">
        <app-header></app-header>
        <div class="quote-form"></div>
        <div class="quote-cards"></div>
        <footer></footer>
    </div>
</template>

<script>
    import Header from './components/Header.vue'

    export default {
        components: {
            appHeader: Header
        }
    }

</script>

<style lang="scss">

</style>
