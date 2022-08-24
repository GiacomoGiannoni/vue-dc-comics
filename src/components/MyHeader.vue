<template>
    <header>
        <img src="@/assets/img/dc-logo.png">
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index" >
                    <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
    export default {
        name: 'MyHeader',
        data() {
            return {
                links: [
                    {
                        text: 'CHARACTERS',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'COMICS',
                        url: '#',
                        active: true
                    },
                    {
                        text: 'MOVIES',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'TV',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'GAMES',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'COOLLECTIBLES',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'VIDEOS',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'FANS',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'NEWS',
                        url: '#',
                        active: false
                    },
                    {
                        text: 'SHOP',
                        url: '#',
                        active: false
                    }

                ] 
            }
        }
    }
</script>

<style lang="scss">
    @import '../style/vars.scss';
    @import '../style/mixin.scss';

    header {
        @include centra('entrambi');
        @include spaziatura('spalbetween');
        margin-left: 100px;
        margin-right: 100px;

        ul {
            list-style: none;
            margin: 20px;
            font-size: 12px;

            li{
                display: inline-block;
                margin: 0px 10px;

                a {
                    color: black;
                    text-decoration: none;
                    padding: 10px;
                    padding-bottom: 40px;
                    font-weight: bold;

                    &.active, &:hover {
                        border-bottom: 3px solid $brand-color;
                        color: $brand-color; 
                    }
                }
            }

        }

    }
</style>