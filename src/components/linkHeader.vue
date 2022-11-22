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
            padding: 1rem;
            margin: 1rem;
           
            a{
                color: #46416A;
                font-weight: 700;
                &:hover{
                color:#20AD96;
            }
                i{
                    padding-left: 0.5rem;
                   }
            }   
            
        }

</style>
