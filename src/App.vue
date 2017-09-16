<template>
    <div id="app">
        <app-header></app-header>
        <quote-form></quote-form>
        <div id="quote-cards">
            <quote-card v-for="n in 10"></quote-card>
        </div>
        <footer></footer>
    </div>
</template>

<script>
    import Header from './components/Header.vue'
    import QuoteForm from './components/QuoteForm.vue'
    import QuoteCard from './components/QuoteCard.vue'

    export default {
        components: {
            appHeader: Header,
            quoteForm: QuoteForm,
            quoteCard: QuoteCard
        }
    }

</script>

<style lang="scss">
    #app {
        margin: 0 10%;
    }
</style>
