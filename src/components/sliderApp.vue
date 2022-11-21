<script >


export default{
    name:"sliderApp",
    props:{
       
    }
}
</script>

<template>
    <span class="slider">slider</span>
    <div class="text-slider flex ">
        <h4 class="text-colored">REAL STORIES</h4>
        <p>I am free to learn a t my own pace, follow my own schedule and choose the subjecxt i want to learn from the syllabus. Great study portal for people like me. 
        </p>
        <img src="../assets/img/testimonial-avata-02.jpg" alt="">
        <h2>Mina Hollace</h2>
        <span>/Freelancer</span>
    </div>
    <div class="img-slider">
        <img src="../assets/img/home-movation-testimonial-image.jpg" alt="">
    </div>
</template>

<style lang="scss" >
.slider{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: red;
    padding: 1rem;
    line-height: 1rem;
    border-radius: 50%;
    width: 50px;
    height: 50px;
}
.text-slider{
    background-image: url(../assets/img/background-pattern-wavify.png);
    width: 50%;
    text-align: center;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    h4{
        font-size: 1rem;
        padding: 1rem;
    }
    p{
        width: 50%;
        font-size: 2rem;
        padding: 1rem;

    }
    img{
        width: 10%;
        border-radius: 50%;
        padding: 1rem;

    }

    span{
        color: grey;
    }
}

.img-slider{
    width: 50%;
    img{
        object-fit: cover;
        width: 100%;
        height: 100%;
    }
}
</style>
