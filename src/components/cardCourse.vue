<script >
import { stringifyExpression } from '@vue/compiler-core';

export default{
    name:"cardCourse",
    props:{
        image: String,
        price: String,
        cent: String,
        title: String,
        lessons: String,
        students: String,

    }
}
</script>

<template>
    <div class="card">
        <img :src="image" alt="">
        <div class="text-card">
            <h2 class="text-colored medium">{{price}}<span class="small">{{cent}}</span> </h2>
            <h3 >{{title}}</h3>
            <div class="lessons-student flex">
                <p><i class="fa-regular fa-file-lines"></i> {{lessons}} </p>
                <p><i class="fa-regular fa-user"></i> {{students}} </p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" >

.card{
    width: calc(100% / 3 - 2rem);
    margin: 2rem 1rem;
    text-align: start;
    overflow: hidden;
    &:hover{
        box-shadow: 2px 2px  10px  grey, -2px -2px  10px  grey;
        img{

            &:hover{
                transform: scale(1.1);
            }
        }
    }
    .text-card{
        
        .medium{
            font-size: 2rem;
            font-weight: 1000;
            padding: 1rem;
        }
        h3{
            width: 80%;
            color:black;
            font-size: 1.5rem;
            padding: 1rem;

        }
        .lessons-student{
            padding: 1rem;
            p{
                padding-right: 1rem;
            }
        }
    }
    
}
</style>
