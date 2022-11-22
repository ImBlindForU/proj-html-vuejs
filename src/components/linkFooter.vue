<script >
export default{
    name:"linkFooter",
    props:{
            linkfooter: String,
        },
           

}
</script>

<template>
    <li class="footer-link"  ><a href="">{{linkfooter}}</a> </li>
</template>

<style lang="scss" >
.footer-link{
    a{
        color: rgb(83, 83, 83);
        &:hover{
            color: #20AD96;
            border-bottom: 1px solid #20AD96;
        }
    }
}
</style>
