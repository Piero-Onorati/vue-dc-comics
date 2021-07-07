<template>
    <header>
        <!-- start  top-header -->
        <div class="container top-header">
            <!-- Logo -->
            <a href="#">
                <img src="../assets/img/dc-logo.png" alt="logo">
            </a>

            <!-- NAV menu -->
            <nav>
                <ul>
                    <li v-for="(link,index) in links" :key="index" :class="{ active: link.selected }">
                        <a :href="link.url" :class="{ active: link.selected }">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
        <!-- end top-header -->

        <!-- Jumbotron -->
        <div class="jumbotron"></div>
    </header>

</template>

<script>
import NavLinks from '@/data/NavLinks.js'
export default {
    name:'Header',
    data(){
        return{
            links:NavLinks
        }
    }

}
</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';

.top-header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    height:90px;

    a{
        img{
            width: 70px;
        }
    }

    nav{

        li{
        display: inline-block;
        line-height: 86px;
        margin: 0 15px;
        
            &:hover,
            &.active{
                color:$primary;
                border-bottom:4px solid $primary;
            }

            a{
                display: inline-block;
                color: $dark;
                font-size:$fsize-sm;
                font-weight: $weight-font;
                text-transform: uppercase;
                text-decoration: none;

                &:hover,
                &.active{
                    color:$primary;
                }
            }
        }
    }
}

.jumbotron{
    height: 320px;
    background-image: url('../assets/img/jumbotron.jpg');
    background-size: cover;
}

</style>