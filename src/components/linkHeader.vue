<script >
export default{
    name:"linkHeader",
    props:{
            link: String,
        },
           

}
</script>

<template>
    <li  ><a href="">{{link}}<i class="fa-solid fa-angle-down"></i></a> </li>
</template>

<style lang="scss" >
 li{
           
           
            a{
                color: #46416A;
                font-weight: 700;
                &:hover{
                color:#20AD96;
                border-bottom: 1px solid #20AD96;

            }   
                i{
                   
                   }
            }   
            
        }

</style>
