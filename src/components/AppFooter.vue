<script >
export default{
    name:"AppFooter"
}
</script>

<template>
    <!-- header top -->
    <div class="container-fluid black mt pt">
        <div class="container flex ">
            <!-- adress -->
            <div class="address list">
                <h4>Address</h4>
                <ul>
                    <li><a href="">382 NE 191st St #87394 Miami, FL 33179-3899</a> </li>
                    <li><a href="">+1[305] 547-9909(9am- 5pm EST, Monday - Friday)</a> </li>
                    <li><a href="">support@maxcoach.com</a> </li>
                    <li class="flex">
                        <a href=""></a>
                        <a href=""></a>
                        <a href=""></a>
                        <a href=""></a>
                    </li>
                </ul>
            </div>
       
        <!-- explore -->
        <div class="flex">
            <div class="explore list">
                <h4>Explore</h4>
                <ul>
                    <li><a href="">Start here</a> </li>
                    <li><a href="">Blog</a> </li>
                    <li><a href="">About us</a> </li>
                    <li><a href="">Success story</a></li>
                    <li><a href="">Course</a></li>
                    <li><a href="">Contact us</a></li>

                </ul>
            </div>
                <div class="information list">
                    <h4>Explore</h4>
                    <ul>
                        <li><a href="">Membership</a> </li>
                        <li><a href="">Purchase guide</a> </li>
                        <li><a href="">Privacy policy</a> </li>
                        <li><a href="">Terms of service</a></li>
                    </ul>
                </div>
            </div>
        </div>    
    </div>
    <!-- header bottom -->
<div class="container-fluid black relative pt">
    <div class="right flex center">
        <p>2020 Maccoach. All Rights Reserved</p>
        
    </div>
    <div class="arrow-up">
       <a href="">arrow</a> 
    </div>
</div>
   
</template>

<style lang="scss" scoped>
.black{
    background-color: #171621;
    min-height: 150px;
}
.address{
    width: 50%;
}
.explore{
    width: 50%;
}
.list{
    h4{
        color:white;
    }
    ul{
        li{
            padding-top: 1rem;
            a{
                color: grey;
            }
        }
    }
}
.center{
    justify-content: center;
    align-items: center;
    color: grey;
}
.arrow-up{
    position: absolute;
    right: 2rem;
    bottom:0;
    background-color: #20AD96;
    border-radius: 50%;
    width: 4rem;
    height: 4rem;
    line-height: 4rem;
    text-align: center;
    margin-bottom: 1rem;

    a{
        color: white;
    }
}
</style>
