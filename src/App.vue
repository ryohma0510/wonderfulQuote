<template>
    <div id="app">
        <app-header></app-header>
        <quote-form></quote-form>
        <div class="quote-cards"></div>
        <footer></footer>
    </div>
</template>

<script>
    import Header from './components/Header.vue'
    import QuoteForm from './components/QuoteForm.vue'

    export default {
        components: {
            appHeader: Header,
            quoteForm: QuoteForm
        }
    }

</script>

<style lang="scss">
    #app {
        margin: 0 10%;
    }

</style>
