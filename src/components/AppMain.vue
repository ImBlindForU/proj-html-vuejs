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

            currentSlider:0,
            slideNumber: 1,
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
                    "newsTitle":"5 Vital Lessons in 5 years of Freelancing",
                    "newsText":"Being self-employed and woriking from home,it's easy to get..."
                },
                {
                    "img":"src/assets/img/motivation-blog-02-480x325.jpg",
                    "date":"May 13,2020",
                    "newsTitle":"11 Super Useful Tips for Small-Buisness Owners",
                    "newsText":"Being a small-business owner poses a ton of challanges. We..."
                },
                {
                    "img":"src/assets/img/motivation-blog-01-480x325.jpg",
                    "date":"May 13,2020",
                    "newsTitle":"How to Give Yourself Grace to Start Again",
                    "newsText":"Forgive yourself for bad habits you may have started or..."
                },
                
            ],
            testimonials:[
                {
                    testimonialWords:"I need to get certification for English proficency and MaxCoach is my best pchoice.Their tutors are smart and professional when dealing with students",
                    testimonialImg:"src/assets/img/testimonial-avata-04.jpg",
                    testimonialName:"Madley Pondor",
                    testimonialWork:"/IT Specialist",
                    testiImage:"src/assets/img/home-movation-testimonial-image.jpg"
                },
                {
                    testimonialWords:"I am free to learn a t my own pace, follow my own schedule and choose the subjecxt i want to learn from the syllabus. Great study portal for people like me.",
                    testimonialImg:"src/assets/img/testimonial-avata-02.jpg",
                    testimonialName:"Mina Hollace",
                    testimonialWork:"/Freelancer",
                    testiImage:"src/assets/img/home-movation-testimonial-image.jpg"

                },
                {
                    testimonialWords:"I am happy with their arragement of lessons and subject. They reflct a scientific investigation into effective methods to adopt for learners",
                    testimonialImg:"src/assets/img/testimonial-avata-01.jpg",
                    testimonialName:"Ludvic Dubble",
                    testimonialWork:"/Private Tutor",
                    testiImage:"src/assets/img/home-movation-testimonial-image.jpg"

                },
                {
                    testimonialWords:"I'm a very stric person so i require everything to be organized and neat. Then, I'll be able to meake things right and shine. MaxCoach guys just got me",
                    testimonialImg:"src/assets/img/testimonial-avata-03.jpg",
                    testimonialName:"Florence Themes",
                    testimonialWork:"/Multimedia Admin",
                    testiImage:"src/assets/img/home-movation-testimonial-image.jpg"

                }

            ],
            
           
        }
    },
    methods:{
        slidedown() {
            if (this.currentSlider < this.testimonials.length - 1) {
                this.currentSlider++;
                this.slideNumber++;
                
            } else {
                this.currentSlider = 0;
                this.slideNumber = 1;
                
            }
        },
        slideUp() {

                if ( this.currentSlider > 0) {
                    this.currentSlider--;
                    this.slideNumber--;

                } else {
                        this.currentSlider = this.testimonials.length - 1;
                        this.slideNumber = this.testimonials.length ;
                        }
                    },
                    

            },

        
    
}
</script>

<template>
    <div class="container-fluid">
        <!-- data  -->
        <section>
            <div class="container mt flex space-between level" >
                <div class="data-container">  
                        <h2 class="text-colored count" >1.926</h2>
                        <h3>FINISHED SESSIONS</h3>
                </div>
                <div class="data-container">  
                        <h2 class="text-colored" >100%</h2>
                        <h3>SATISFACTION RATE</h3>
                </div>
                <div class="data-container">  
                        <h2 class="text-colored " >3092+</h2>
                        <h3>ENROLLED LEARNERS</h3>
                </div>
                <div class="data-container">  
                        <h2 class="text-colored " >200</h2>
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
                    <h2 class="text-purple">Kaixa Stark</h2>
                    <h4 class="text-purple">WINGMAN</h4>
                </div>
            </div>
        </section>
        <!-- latest course -->
        <section>
            <div class="container mt ">
                <div class="text-course">
                    <h4>BEGIN YOUR JOURNEY AT MAXCOACH</h4>
                    <h2 class="text-purple">Latest <span class="text-colored">Online Courses</span></h2>
                    <div class="row-cards flex wrap">
                        <cardCourse v-for="(card, index) in cards" :key="index"
                                    :image="card.image"
                                    :price="card.price"
                                    :cent="card.cent"
                                    :title="card.title"
                                    :lessons="card.lessons"
                                    :students="card.students"/>
                                     
                    </div>
                    <button ><a href="">View all courses</a>  </button>
                </div>
            </div>
        </section>

        <!-- book section -->
        <section>
            <div class="container mt flex">
                <div class="book-store-text">
                    <h4 class="text-darkgrey">BOOK STORE ONLINE</h4>
                    <h2 class="text-purple">Be Alpha With <span class="text-colored">Wingman's Book</span></h2>
                    <ul class="text-grey">
                        <li><i class="fa-solid fa-check"></i>Help you understand yourself better</li>
                        <li><i class="fa-solid fa-check"></i>Revealing mature tips</li>
                        <li><i class="fa-solid fa-check"></i>Give the right advice</li>
                        <li><i class="fa-solid fa-check"></i>Fascinating exeples of alpha man</li>
                    </ul>
                    <button><a href="">Get Free Ebook</a> </button>
                </div>
                <div class="books flex">
                    <div class="book relative">
                        <img src="../assets/img/product-book-11-400x400.jpg" alt="">
                        <div class="text-book">
                            <h4>Alpha man by Maxcoach</h4>
                            <h4 class="text-colored"> $29<span class="small">.00</span> </h4>
                        </div>
                        <!-- <div class="hover-list">
                            <ul>
                                <li>
                                   <span class="opacity">Click view</span> <i class=" opacity fa-solid fa-magnifying-glass"></i>
                                </li>
                                <li>
                                    <span class="opacity">shop</span><i class=" opacity fa-solid fa-cart-shopping"></i>
                                </li>
                                <li>
                                    <span class="opacity">Add to whishlist</span><i class="opacity fa-regular fa-heart"></i>
                                </li>
                                <li>
                                     <span class="opacity">Compare</span><i class="opacity fa-solid fa-signal"></i>
                                </li>
                            </ul>
                        </div> -->
                    </div>
                    <div class="book relative">
                        <img src="../assets/img/product-book-10-400x400.jpg" alt="">
                        <div class="text-book">
                            <h4>Real man 4.0 by Maccoach</h4>
                            <h4 class="text-colored">$39<span class="small">.00</span></h4>
                        </div>
                        <!-- <div class="hover-list">
                            <ul>
                                <li>
                                   <span class="opacity">Click view</span> <i class=" opacity fa-solid fa-magnifying-glass"></i>
                                </li>
                                <li>
                                    <span class="opacity">shop</span><i class=" opacity fa-solid fa-cart-shopping"></i>
                                </li>
                                <li>
                                    <span class="opacity">Add to whishlist</span><i class="opacity fa-regular fa-heart"></i>
                                </li>
                                <li>
                                     <span class="opacity">Compare</span><i class="opacity fa-solid fa-signal"></i>
                                </li>
                            </ul>
                        </div> -->
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
    <div class="container-fluid mt reviews flex relative wrap">
        <div class="slide flex">
                <div class="slider flex">
                    <span  @click="slideUp"><i class="fa-solid fa-caret-up"></i> </span>
                    <span> {{slideNumber}}/4</span>
                    <span @click="slidedown"><i  class="fa-solid fa-caret-down"></i></span>
                </div>
                <div  class="text-slider flex ">
                    <h4 class="text-colored">REAL STORIES</h4>
                    <p>{{testimonials[currentSlider].testimonialWords}}
                    </p>
                    <img :src="testimonials[currentSlider].testimonialImg" alt="">
                    <h2>{{testimonials[currentSlider].testimonialName}}</h2>
                    <span>{{testimonials[currentSlider].testimonialWork}}</span>
                </div>
                <div class="img-slider">
                    <img src="../assets/img/home-movation-testimonial-image.jpg" alt="">
                </div>
        </div>



    </div>

    <!-- blog udate -->
    <div class="container-fluid mt relative">
        <div class="container">
            <h4>BLOG UPDATE</h4>
            <h2>Interesting <span class="text-colored">articles updated</span> daily</h2>
            <div class="newses-list flex wrap spac-between">
                <newsApp  v-for="(news, index) in newses"  :key="index"
                :img="news.img"
                :date="news.date"
                :newsText="news.newsText"
                :newsTitle="news.newsTitle"
                 />
                 <span class="view-all">
                    VIEW ALL POSTS
                </span>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
// data
.data-container{
    background-image: url(../assets/img/background-pattern-grid-line-06.png);
    background-position: left;
    background-repeat: no-repeat;
    padding-left: 3rem;
    h2{
       
        text-align: center;
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
    overflow: hidden;
    &:hover{
        transform: scale(1.1);
    }
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

        padding-top: 1rem;
    }
}

// book store
// .hover-list{
//     position: absolute;
//     top: 10%;
//     right: 10%;
//     ul{
//         li{
//            text-align: end;
//             i{
//                 background-color: white;
//                 border-radius: 50%;
              
//                 &:hover{
                    
//                     background-color: #20AD96;
//                 }
//             }
//         }
//     }
// }
.book-store-text{
    width: 40%;
    h2{
        width: 60%;
    }
    ul {
        li{
           
          
            i{
               padding-right: 0.5rem;
                color: #20AD96;
               
            }
        }
    }
    button{
        margin-top: 1rem;
    }
}

.book{
    overflow: hidden;
    text-align: center;
    img{
        padding-right: 2rem;
        padding-top: 2rem;
        &:hover{
            transform: scale(1.1);
        }
       
    }
    h4{
        padding-top: 1rem;
        
    }
    
}

// sponsor

.sponsor{
    color: #20AD96;
    filter: grayscale(90%);
    opacity: 0.3;
}

// slider
.slide{
    width: 100%;
}
.slider{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: white;
    border: 1px solid rgba(187, 181, 181, 0.726);
    line-height: 25px;
    border-radius: 50%;
    width: 100px;
    height: 100px;
    max-width: 150px;
    max-height: 150px;
    text-align: center;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    i{
        color: #D5D5D5;
        font-size: 1rem;
    }

}
.text-slider{
    background-image: url(../assets/img/background-pattern-wavify.png);
    background-color: #F2F2F9;
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

// blog
.view-all{
        margin-left: 50%;
        transform: translate(-50%);
        text-align: center;
        color: #20AD96;
        margin-top: 3rem;
        border-bottom: 1px solid #20AD96;

    }

</style>
