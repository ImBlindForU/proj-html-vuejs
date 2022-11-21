<script >


export default{
    name:"sliderApp",
    props:{
        testimonialWords: String,
        testimonialImg: String,
        testimonialName: String,
        testimonialWork: String,
    },
    emits: ['parentUp', 'parentDown'],
   
}
</script>

<template>
    <div class="slider flex">
        <span  @click="$emit('parentUp')"><i class="fa-solid fa-caret-up"></i> </span>
        <span> /4</span>
        <span @click="$emit('parentDown')"><i  class="fa-solid fa-caret-down"></i></span>
    </div>
    <div class="text-slider flex ">
        <h4 class="text-colored">REAL STORIES</h4>
        <p>{{testimonialWords}}
        </p>
        <img src="testimonialImg" alt="">
        <h2>{{testimonialName}}</h2>
        <span>{{testimonialWork}}</span>
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
    background-color: white;
    border: 1px solid black;
    line-height: 25px;
    border-radius: 50%;
    width: 200px;
    height: 200px;
    max-width: 150px;
    max-height: 150px;
    text-align: center;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    

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
