<script >


export default{
    name:"newsApp",
    props:{
        img: String,
        date: String,
        newsText: String,
        newsTitle: String,
    }
}
</script>

<template>
 <div class="news">
    <img :src="img" alt="">
    <div class="text-news">
        <p>{{date}}</p>
        <h4>{{newsTitle}}</h4>
        <p>{{newsText}}</p>
    </div>
 </div>
</template>

<style lang="scss" >
.news{
    width: calc(100% / 4 - 2rem );
    margin: 1rem;
    
}

</style>
