<script >
import cardCourse from "./cardCourse.vue"
import newsApp from "./newsApp.vue"

export default{
    name:"AppMain",
    components:{
        cardCourse,
        newsApp,
    },
    data(){
        return{

            cards:[
                {
               
                    "image":"src/assets/img/motivation-course-06-480x298.jpg",
                    "price":"$20",
                    "cent":".00",
                    "title":"How to be Successful:Create A Growth Mindset For Success",
                    "lessons":"3 Lesson",
                    "students":"50 Students"
                },
                {

                    "image":"src/assets/img/motivation-course-05-480x298.jpg",
                    "price":"$30",
                    "cent":".00",
                    "title":"How to Build Confidance in Your Abilities",
                    "lessons":"1 Lesson",
                    "students":"50 Students"
                },
                {

                    "image":"src/assets/img/motivation-course-04-480x298.jpg",
                    "price":"$20",
                    "cent":".00",
                    "title":"Productivity Machine - focus in a Distracted World",
                    "lessons":"5 Lesson",
                    "students":"50 Students"
                },
                {
               
                    "image":"src/assets/img/motivation-course-03-480x298.jpg",
                    "price":"$20",
                    "cent":".00",
                    "title":"Effective Time Managemente Mastery - Complete Guide",
                    "lessons":"18 Lesson",
                    "students":"50 Students"
                },
                {

                    "image":"src/assets/img/motivation-course-02-480x298.jpg",
                    "price":"$25",
                    "cent":".99",
                    "title":"Body Language Secrets for Entrepreneurs",
                    "lessons":"19 Lesson",
                    "students":"50 Students"
                 },
                {

                    "image":"src/assets/img/motivation-course-01-480x298.jpg",
                    "price":"$19",
                    "cent":".99",
                    "title":"Management Sills: The Science of Leadership",
                    "lessons":"17 Lesson",
                    "students":"50 Students"
                }
            ],
            newses:[
                {
                    "img":"src/assets/img/motivation-blog-04-480x325.jpg",
                    "date":"May 13,2020",
                    "newsTitle":"How to Stay True To Your Personal Brand",
                    "newsText":"When it comes to your buismess or career,you want..."
                },
                {
                    "img":"src/assets/img/motivation-blog-03-480x325.jpg",
                    "date":"May 13,2020",
                    "newsTitle":"How to Stay True To Your Personal Brand",
                    "newsText":"When it comes to your buismess or career,you want..."
                },
                {
                    "img":"src/assets/img/motivation-blog-02-480x325.jpg",
                    "date":"May 13,2020",
                    "newsTitle":"How to Stay True To Your Personal Brand",
                    "newsText":"When it comes to your buismess or career,you want..."
                },
                {
                    "img":"src/assets/img/motivation-blog-01-480x325.jpg",
                    "date":"May 13,2020",
                    "newsTitle":"How to Stay True To Your Personal Brand",
                    "newsText":"When it comes to your buismess or career,you want..."
                },
                
            ],

        }
    }
}
</script>

<template>
    <div class="container-fluid">
        <!-- data  -->
        <section>
            <div class="container mt flex space-between" >
                <div class="data-container">  
                        <h2 class="text-colored">1.926</h2>
                        <h3>FINISHED SESSIONS</h3>
                </div>
                <div class="data-container">  
                        <h2 class="text-colored">100%</h2>
                        <h3>SATISFACTION RATE</h3>
                </div>
                <div class="data-container">  
                        <h2 class="text-colored">3092+</h2>
                        <h3>ENROLLED LEARNERS</h3>
                </div>
                <div class="data-container">  
                        <h2 class="text-colored">200</h2>
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
                        <h4>Want to learn hot to be <span class="text-colored">an alpha male</span>?How to be more masculine?How to be the man you've always wanted to be?</h4>
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
            <div class="container mt ">
                <div class="text-course">
                    <h4>BEGIN YOUR JOURNEY AT MAXCOACH</h4>
                    <h2>Latest <span class="text-colored">Online Courses</span></h2>
                    <div class="row-cards flex wrap">
                        <cardCourse v-for="(card, index) in cards" :key="index"
                                    :image="card.image"
                                    :price="card.price"
                                    :cent="card.cent"
                                    :title="card.title"
                                    :lessons="card.lessons"
                                    :students="card.students" />
                                     
                    </div>
                    <button ><a href="">View all courses</a>  </button>
                </div>
            </div>
        </section>

        <!-- book section -->
        <section>
            <div class="container mt flex">
                <div class="book-store-text">
                    <h4>BOOK STORE ONLINE</h4>
                    <h2>Be Alpha With <span class="text-colored">Wingman's Book</span></h2>
                    <ul>
                        <li>Help you understand yourself better</li>
                        <li>Revealing mature tips</li>
                        <li>Give the right advice</li>
                        <li>Fascinating exeples of alpha man</li>
                    </ul>
                    <button><a href="">Get Free Ebook</a> </button>
                </div>
                <div class="books flex">
                    <div class="book">
                        <img src="../assets/img/product-book-11-400x400.jpg" alt="">
                        <div class="text-book">
                            <h2>Alpha man by Maxcoach</h2>
                            <h2 class="text-colored"> $29<span class="small">.00</span> </h2>
                        </div>
                    </div>
                    <div class="book">
                        <img src="../assets/img/product-book-10-400x400.jpg" alt="">
                        <div class="text-book">
                            <h2>Real man 4.0 by Maccoach</h2>
                            <h2 class="text-colored">$39<span class="small">.00</span></h2>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- sponsor -->
        <section>
            <div class="container mt">
                <div class="sponsors flex space-between">
                    <div class="sponsor">
                        <img src="../assets/img/client-logo-05-primary.png" alt="">
                    </div>
                    <div class="sponsor">
                        <img src="../assets/img/client-logo-06-primary.png" alt="">
                    </div>
                    <div class="sponsor">
                        <img src="../assets/img/client-logo-07-primary.png" alt="">
                    </div>
                    <div class="sponsor">
                        <img src="../assets/img/client-logo-04-primary.png" alt="">
                    </div>
                    <div class="sponsor">
                        <img src="../assets/img/client-logo-03-primary.png" alt="">
                    </div>
                    <div class="sponsor">
                        <img src="../assets/img/client-logo-02-primary.png" alt="">
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- recensioni -->
    <div class="container-fluid mt reviews">
        <div class="text-revieww">
            <!-- rewis slider -->a
        </div>
    </div>

    <!-- blog udate -->
    <div class="container-fluid mt">
        <div class="container">
            <h4>BLOG UPDATE</h4>
            <h2>Interesting <span class="text-colored">articles udated</span> daily</h2>
            <div class="newses-list flex wrap spac-between">
                <newsApp v-for="(news, index) in newses" :key="index"
                :img="news.img"
                :date="news.date"
                :newsText="news.newsText"
                :newsTitle="news.newsTitle" />
            </div>
        </div>
    </div>
</template>

<style lang="scss">
// data
.data-container{
    background-image: url(../assets/img/background-pattern-grid-line-06.png);
    background-position: left;

    padding-left: 3rem;
    h2{
       
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


// card section
.text-course{
    text-align: center;
    h2{
        font-size: 3rem;
        padding-top: 1rem;
    }
}

// book store

.book-store-text{
    width: 40%;
    h2{
        width: 60%;
        font-size: 3rem;
    }
    ul {
        li{
            padding-top: 0.5rem;
            padding-bottom: 0.5rem;
        }
    }
    button{
        margin-top: 1rem;
    }
}

.book{
    text-align: center;
    img{
        padding-right: 2rem;
        padding-top: 2rem;
    }
    h2{
        padding-top: 1rem;
        
    }
    
}

// sponsor

.sponsor{
    filter: grayscale(100%);
    opacity: 0.3;
}

</style>
