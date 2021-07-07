<template>

    <div class="card">
        <div class="img-box">
            <img :src="element.thumb" :alt="element.series">
        </div>
        <span>{{element.series}}</span>
    </div>
  
</template>

<script>
export default {
    name:'Card',
    props: ["element"]

}
</script>

<style lang="scss">

.card{
    width: calc(100% / 6 - 20px);
    margin: 0 10px;
    margin-top: 50px;
    text-align: left;

    .img-box{
        height: 150px;
        overflow: hidden;
        
        img{
            width:100%
        }
    }

    span{
        padding-top: 20px;
        display: block;
        color:white;
        text-transform: uppercase;
        font-size: 14px;
    }
}

</style>