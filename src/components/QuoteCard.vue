<template>
    <div id="quote-card" @click="deleteCard()">
        <slot></slot>
    </div>
</template>

<script>
    export default {
        props: ['quoteId'],
        methods: {
            deleteCard () {
                this.$emit('cardWasClicked', this.quoteId)
            }
        }
    }
</script>

<style scoped lang="scss">
    div {
        border: 1px solid #251d1d;
        border-radius: 10px;
        padding: 10px;
        margin: 10px 10px 0 0;
        display: inline-block;
        cursor: pointer;
        &:hover {
            background-color: rgba(3, 169, 244,0.44);
        }
    }

    p {
        font-family: 'Arizonia', cursive;
        font-size: 40px;
    }
</style>
