<template>
<div class="container">
   <img class="images" src="@/static/background3.jpeg" alt="">
</div>
      
</template>


<script>
export default {
    name: 'P2ImageHeader',

}
</script>

<style lang="scss" scoped>
.container {
    padding: 0;
    margin: 0;
    max-width: 100%;    
}
.images {
    width: 100%;
    height: 700px;
}

@media screen and (max-width: 1420px) {
    .images {
    height: 400px;
}
}  
@media screen and (min-width: 768px) and (max-width: 991px) {
    .images {
    height: 350px;
}
}
@media screen and (max-width: 599px) {
    .container {
        margin-top: 50px;
    }
    .images {
    height: 300px;
}
}
</style>