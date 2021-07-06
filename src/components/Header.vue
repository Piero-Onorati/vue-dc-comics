<template>
    <header class="container header">
        <a href="#">
            <img src="../assets/img/dc-logo.png" alt="logo">
        </a>
        <nav>
            <ul>
                <li v-for="(link,index) in links" :key="index" :class="{ active: link.selected }">
                    <a :href="link.url" :class="{ active: link.selected }">{{link.text}}</a>
                </li>
            </ul>
        </nav>

    </header>
</template>

<script>
export default {
    name:'Header',
    data(){
        return{
            links:[
                {
                    text:'characters',
                    url: '#',
                    selected: false
                },
                {
                    text:'comics',
                    url: '#',
                    selected: true
                },
                {
                    text:'movie',
                    url: '#',
                    selected: false
                },
                {
                    text:'tv',
                    url: '#',
                    selected: false
                },
                {
                    text:'games',
                    url: '#',
                    selected: false
                },
                {
                    text:'collectibles',
                    url: '#',
                    selected: false
                },
                {
                    text:'videos',
                    url: '#',
                    selected: false
                },
                {
                    text:'fan',
                    url: '#',
                    selected: false
                },
                {
                    text:'news',
                    url: '#',
                    selected: false
                },
                {
                    text:'shop',
                    url: '#',
                    selected: false
                }
            ]
        }
    }


}
</script>

<style lang="scss" scoped>
@import '@/style/vars.scss';

.header{
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
        

        &.active{
            color:$primary;
            border-bottom:4px solid $primary;

        }

        a{
            display: inline-block;
            color: $dark;
            font-size:13px ;
            font-weight: $weight-font;
            text-transform: uppercase;
            text-decoration: none;

            &.active{
                color:$primary;

            }
        }
        
        }
    }

    
    

    
    
}

</style>