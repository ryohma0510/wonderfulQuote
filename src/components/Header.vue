<template>
    <div id="header">
        <h2>Quotes Added</h2>
        <div id="bar-box">
            <p>{{ quotesNumber }} / 10</p>
            <div id="bar" :style="{width: barWidth}"></div>
        </div>

    </div>
</template>

<script>
    export default {
        props: ['quotesNumber'],
        computed: {
            barWidth () {
                return (this.quotesNumber * 10).toString() + '%'
            }
        }
    }
</script>

<style scoped lang="scss">
    h2 {
        padding: 0px 0px 0px 20px;
    }

    #bar-box {
        height: 40px;
        border-radius: 20px;
        background-color: #ccc;
        position: relative;
        p {
            position: absolute;
            left: 50%;
        }
    }

    #bar {
        height: 100%;
        text-align: center;
        line-height: 200%;
        border-radius: 20px;
        background-color: rgba(3, 169, 244,0.44);
        position: absolute;
    }
</style>
