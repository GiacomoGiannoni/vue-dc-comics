<template>
    <div class="comic">
        <div class="comics-img">
            <img :src="fumetti.thumb">
        </div>
        <h4>{{fumetti.series}}</h4>
    </div>
</template>

<script>
export default {
    name: 'CardComics',
    props: {
        fumetti: Object,
    }
}
</script>

<style lang="scss">
    @import '../style/mixin.scss';

    .comics {
        display: flex;
        @include spaziatura('spalbetween');
        flex-wrap: wrap;

        .comic {
            width: calc(100% / 6 - 1rem);

            .comics-img {
                width: 100%;
                height: 200px;

                img{
                    width: 100%;
                    height: 100%;
                    background-size: contain;
                }
            }
        }
    }
</style>
