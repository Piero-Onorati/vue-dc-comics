<template>
    <section>
        <div class="container content-box">
            <ul>
                <li v-for="(item,index) in items" :key="index">
                    <div class="img-box">
                        <img :src="require('../assets/img/'+ item.image)">
                    </div>
                    <span>{{item.didascalia}}</span>
                </li>
            </ul>
        </div>
        
    </section>
  
</template>

<script>
import HighlightedContentData from '@/data/HighlightedContentData.js'

export default {
    name:'HighlightedContent',
    data(){
        return{
            items:HighlightedContentData
        }
    }
}


</script>

<style lang='scss' scoped>
@import '@/style/vars.scss';

section{
    padding: 50px 0;
    background-color: $primary;

    ul{
    display: flex;
    align-items:center ;
    justify-content: space-around;

    li{
        display:flex;
        align-items: center;

        .img-box{
            height: 50px; 
            margin-right: 8px;

            img{
                height: 50px;
            }
        }

        span{
            color:white;
            text-transform: uppercase;
            font-size: 14px;
        }
        
    }
    
}
}

</style>