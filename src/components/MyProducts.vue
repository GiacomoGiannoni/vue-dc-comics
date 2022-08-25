<template>
    <main>
        <div class="products container">
            <h2>Content goes here</h2>
        </div>
    </main>
</template>

<script>
    export default {
        name: 'MyProducts'
    }
</script>

<style scoped lang="scss">
    @import '../style/mixin.scss';
    @import '../style/mixin.scss';

    main {
        background-color: black;
    }
    .products {
        @include spaziatura('spalbetween');
        color: white;
        line-height: 100px;
        height: 100px;
    }
</style>