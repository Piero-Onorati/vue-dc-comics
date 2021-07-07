<template>
    <section>
        <div class="container">
            <!-- Label -->
            <span class="label">current series</span>

            <!-- Box with all the comics -->
            <div class="books-box">
                <Card v-for="(book,index) in books" :key="index" :element="book"/>
            </div>

            <!-- Button -->
            <span class="button">Load More</span>
        </div>
    </section>
</template>

<script>

import Comics from '@/data/Comics.js';
import Card from './Card.vue'

export default {
    name:'MainContent',
    components: {
        Card,
    },
    data(){
        return{
            books: Comics
        }
    }

}
</script>

<style lang='scss' scoped>
@import '@/style/vars.scss';


section{
    background-color: $darkest;
    text-align: center;

    .container{
        position: relative;

        .label{
            position: absolute;
            top:-16px;
            left: 0px;
            font-size:$fsize-md ;
            font-weight: $weight-font;
            background-color: $primary;
            text-transform: uppercase;
            padding: 6px 25px;
            color:white;
        }

        .books-box{
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
        }

        .button{
            margin: 50px 0 25px 0;
            padding: 5px 50px;
            font-size:$fsize-sm ;
            font-weight: $weight-font;
            text-transform: uppercase;
            display: inline-block;
            background-color: $primary;
            color:white
        }

    }
}

</style>