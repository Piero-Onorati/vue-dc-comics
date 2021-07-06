<template>
    <section>
        <div class="container">
            <h2>-->Contents goes here>--- </h2>
        </div>
    </section>
</template>

<script>
export default {
    name:'MainContent'

}
</script>

<style lang='scss' scoped>
@import '@/style/vars.scss';

section{
    height: 120px;
    background-color: $darkest;

    h2{
        padding:40px 0;
        color:white
    }
}

</style>