<template>
    <div id="app">
        <app-header :quotesNumber="quotes.length"></app-header>
        <app-quote-form  @quoteWasAdded="quotes.push($event)"></app-quote-form>
        <div id="quote-cards">
            <app-quote-card v-for="quote in quotes" :quote="quote"></app-quote-card>
        </div>
        <app-footer></app-footer>
    </div>
</template>

<script>
    import Header from './components/Header.vue'
    import QuoteForm from './components/QuoteForm.vue'
    import QuoteCard from './components/QuoteCard.vue'
    import Footer from './components/Footer.vue'


    export default {
        data () {
            return {
                quotes: ['great', 'wonderful', 'excellent']
            }
        },
        components: {
            appHeader: Header,
            appQuoteForm: QuoteForm,
            appQuoteCard: QuoteCard,
            appFooter: Footer
        }
    }

</script>

<style lang="scss">
    #app {
        margin: 0 10%;
    }
    #quote-cards {
        margin-top: 20px;
    }
</style>
