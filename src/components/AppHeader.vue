<script >

export default{
    name:"AppHeader",
    data(){
        return{
            headerLinks:{
                    home: "Home",
                    pages:"Pages",
                    course:"Course",
                    features:"Features",
                    blog:"Blog",
                    shop:"Shop"
            },
            icons:[
                
            ]
            
  
        }  
    }
}
</script>

<template>

    <div class="container-fluid backgroundimg">
        <!-- general bar -->
        <div class="container flex space-between header-heigt">
            <div class="logo">
                <img src="../assets/img/dark-logo.png" alt="">
            </div>
            <div class="list-general ">
                <ul class="flex space-between">
                    <li  v-for="(headerLink, index) in headerLinks" :key="index"><a href="">{{headerLink}}</a> </li>
                </ul>
            </div>
            <div class="icons">
                <ul>
                    <li></li>
                </ul>
            </div>
        </div>
        <!-- jumbotron -->
        <div class="container flex relative">
            <div class="mini-menubar ">
               <div class="tool">
                    a
               </div>
               <div class="tool">
                    b
               </div>
               <div class="tool"> 
                    c
               </div>
               <div class="tool">
                    d
               </div>
            </div>
            <div class="jumbo-text flex">
                <h2>I'M WINGMAN</h2>
                <h1>Peace On Earth A Wonderful Wish But No Way</h1>
                <p>Success isn't overnight. it's when everyday you get a little better than the day before. It all adds up</p>
                <button><a href=""> Get Started For Free  arrowleft</a></button>
            </div>
            <div class="jumbo-img">
                <img src="../assets/img/home-movation-hero-image.png" alt="">
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

.header-heigt{
    height: 100px;
}
.backgroundimg{
    background-image: url(../assets/img/background-pattern-wavify.png);
}

.list-general{
    ul{
        li{
            padding: 2rem;
            margin: 1rem;
            a{
                color: #46416A;
                font-weight: 700;
            }   
            
        }
    }
}
.jumbo-text{
    width: 40%;
    flex-direction: column;
    justify-content: center;
    h2{
        font-size: 2rem;
        padding-bottom: 1rem;
    }
    h1{

        font-size: 4rem;
        padding-bottom: 1rem;

    }
    p{
        font-size: 1.5rem;
        padding-bottom: 1rem;

    }
    button{
        width: 30%;
        padding: 1rem;
    }
}
.jumbo-img{
    width: 60%;
    background-image: url(../assets/img/home-movation-shape-face.png);
    background-position: bottom;
    background-size: contain;
    text-align: center;
    background-repeat:no-repeat;

}

.mini-menubar{
    position: absolute;
    top: 5rem;
    right: 0;
    background-color: grey;

    .tool{
        width: 2rem;
        height: 2rem;
        border: 1px solid black;
        text-align: center;
        vertical-align: middle;
    }
}
</style>
