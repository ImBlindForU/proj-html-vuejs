<script >

import linkFooter from './linkFooter.vue';
export default{
    name:"AppFooter",
    components:{
        linkFooter
},
data(){
        return{
            addresses:{
                adre:"382 NE 191st St #87394 Miami, FL 33179-3899",
                call:"+1[305] 547-9909(9am- 5pm EST, Monday - Friday)",
                support:"support@maxcoach.com"
            },
            explores:{
                        start:"Start here",
                        Blog:"Blog",
                        about:"About us",
                        story:"Success story",
                        course:"Course",
                        Contact:"Contact us"

            },
            informations:{
                Membership:"Membership",
                Purchaseguide:"Purchase guide",
                Privacypolicy:"Privacy policy",
                Termsofservice:"Terms of service"
            }
           
            
  
        }  
    }
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
                    <linkFooter v-for="(address, index) in addresses" :key="index"
                    :linkfooter="address" />
                    <li> 
                        <ul class="flex footer-icons">
                            <li><a href=""> <i class="fa-brands fa-twitter"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-facebook-f"></i></a></li>
                            <li><a href=""><i class="fa-brands fa-instagram"></i></a></li>
                        <li><a href=""><i class="fa-brands fa-linkedin"></i></a></li>
                    </ul>
       
                    </li>
                </ul>
            </div>
       
        <!-- explore -->
       
            <div class="explore list">
                <h4>Explore</h4>
                <ul>
                    <linkFooter v-for="(explore, index) in explores" :key="index"
                    :linkfooter="explore" />

                </ul>
            </div>
                <div class="information list">
                    <h4>Information</h4>
                    <ul>
                        <linkFooter v-for="(information, index) in informations" :key="index"
                        :linkfooter="information" />
                    </ul>
                </div>
            
        </div>    
    </div>
    <!-- header bottom -->
<div class="container-fluid black relative pt">
    <div class="right flex center">
        <p>© 2020 Maccoach. All Rights Reserved</p>
        
    </div>
    <div class="arrow-up">
       <a href=""><i class="fa-solid fa-arrow-up"></i></a> 
    </div>
</div>
   
</template>

<style lang="scss" scoped>
.footer-icons{
    li{
        a{
            i{
                &:hover{
                color: #20AD96;
    }
            }
        }
    }
   
}
.black{
    background-color: #171621;
    min-height: 150px;
}
.address{
    width: 50%;
}

.explore{
    width: 20%;
    height: 10%;
    
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
    color: rgb(170, 170, 170);
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
