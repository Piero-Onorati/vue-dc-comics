<template>
    <section>
        <div class="container content-box">
            <HighlightedContentItem/> 
        </div>
        
    </section>
  
</template>

<script>
import HighlightedContentItem from './HighlightedContentItem.vue'



export default {
    name:'HighlightedContent',
    components:{
        HighlightedContentItem
    }
}


</script>

<style lang='scss' scoped>
@import '@/style/vars.scss';

section{
    padding: 50px 0;
    background-color: $primary;
}

</style>