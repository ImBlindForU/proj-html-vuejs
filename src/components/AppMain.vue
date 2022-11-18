<script >
export default{
    name:"AppMain"
}
</script>

<template>
    <div class="container-fluid">
        <!-- data  -->
        <section>
            <div class="container mt flex space-between" >
                <div class="data-container">  
                        <h2>1.926</h2>
                        <h3>FINISHED SESSIONS</h3>
                </div>
                <div class="data-container">  
                        <h2>100%</h2>
                        <h3>SATISFACTION RATE</h3>
                </div>
                <div class="data-container">  
                        <h2>3092+</h2>
                        <h3>ENROLLED LEARNERS</h3>
                </div>
                <div class="data-container">  
                        <h2>200</h2>
                        <h3>ONLINE INSTRUCTORS</h3>
                </div>
            </div>
        </section>
       
        <!-- about me -->

        <section>
            
            <div class="container mt">
                <h3>ABOUT ME</h3>
                <div class="flex">
                    <div class="title-about-me">
                        <h2>
                            How to Be an Alpha Male : The 15 Habits of True Alphas
                        </h2> 
                    </div>
                    <div class="text-about-me">
                        <h4>Want to learn hot to be <span>an alpha male</span>?How to be more masculine?How to be the man you've always wanted to be?</h4>
                        <p>Your goal is to show the consistency of buisness,care values, and customer care.Punctually,responsability,individuality,accuracy,entusiasm - you have to clearly explain how these qualities are applicable to your work.And the important thing is you do love what do you do</p>
                    </div>  
                </div>
            </div>
            <!-- video section -->
            <div class="container flex mt">
                <div class="youtube-video relative">
                    <span><img src="../assets/img/icon-youtube-play.png" alt=""></span>
                </div>
                <div class="text-video">
                    <h3>
                        "Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them"
                    </h3>
                    <img src="../assets/img/home-movation-shape-01.png" alt="">
                    <h2>Kaixa Stark</h2>
                    <h4>WINGMAN</h4>
                </div>
            </div>
        </section>
        <!-- latest course -->
        <section>
            <div class="container">
                <!-- card dinamic -->
            </div>
        </section>
    </div>
</template>

<style lang="scss">
// data
.data-container{
    background-image: url(../assets/img/background-pattern-grid-line-06.png);
    background-position: left;

    padding-left: 3rem;
    h2{
        color: #20AD96;
        text-align: center;
        font-size: 3rem;
        padding: 1rem;

    }
    h3{
        color:rgba(0, 0, 0, 0.575);
        text-align: center;
    }
}

// about me

h3{
    color: #20AD96;
    font-size: 2rem;
    padding-bottom: 3rem;
 }  
 .title-about-me{
    width: 50%;
    h2{
        width: 60%;
        font-size: 3rem;
    }
 }
 .text-about-me{
    width: 50%;
    h4{
        font-size: 1.5rem;
        padding: 1rem;
        span{
            color: #20AD96;
        }
    }
    p{
        padding: 1rem;
        font-size: 1rem;
    }
 }

//  about me video
.youtube-video{
    width: 50%;
    min-height: 500px;
    background-image: url(../assets/img/home-movation-video-poster-670x450.jpg);
    background-position: center;
    background-size: cover;
    span{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
}
.text-video{
    width: 50%;
    flex-direction: column;
    
    padding-left: 6rem;
    h3{
        width: 70%;
        padding-top: 4rem;
        color: grey;
    }
    img{
        padding-top: 4rem;
    }
    h2{
        padding-top: 1rem;
    }
    h4{
        padding-top: 1rem;
    }
}

</style>
