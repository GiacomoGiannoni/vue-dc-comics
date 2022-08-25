<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="@/assets/img/dc-logo.png">
            </div>
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index" >
                        <a :href="link.url" :class="link.active?'active':''" >{{link.text}}</a>
                    </li>
                </ul>
            </nav>

        </div>
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
        height: 150px;
        padding-top: 10px;

        .logo {
            display: flex;
            align-items: center;
        }

        .container {
            @include spaziatura('spalbetween');
        }

        ul {
            display: flex;
            align-content: center;
            list-style: none;
            height: 100%;

            li{
                display: flex;
                align-items: center;
                list-style: none;
                height: 100%;

                a {
                    color: black;
                    text-decoration: none;
                    height: 100%;
                    line-height: 150px;
                    margin: 0 10px;
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