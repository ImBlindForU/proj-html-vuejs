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
        <p><i class="fa-regular fa-calendar"></i>{{date}}</p>
        <h4>{{newsTitle}}</h4>
        <p>{{newsText}}</p>
    </div>
    
 </div>
</template>

<style lang="scss" >
.news{
    width: calc(100% / 4 - 2rem );
    margin-right: 2rem;
    margin-top: 3rem;
    overflow: hidden;
    &:hover{
        img{

            &:hover{
                transform: scale(1.1);
            }
        }
    }
    .text-news{
        p{
            padding-top: 1rem;
            i{
                padding-right: 0.5rem;
            }
        }
        h4{
            padding-top: 1rem;
            font-weight: 900;
            font-size: 1.5rem;
        }

    }
   
}

</style>
