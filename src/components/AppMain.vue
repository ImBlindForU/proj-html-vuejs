<script >
export default{
    name:"AppMain"
}
</script>

<template>
    <div class="container-fluid">
        <!-- data  -->
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
</style>
