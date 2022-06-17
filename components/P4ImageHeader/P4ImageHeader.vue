<template>
<div class="container">
   <img class="images" src="@/static/background4.jpg" alt="">
</div>
  
</template>

<script>
export default {
    name: 'P4ImageHeader',

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
@media screen and (max-width: 599px) {
    .images {
    height: 200px;
}
}
@media screen and (max-width: 1420px) {
    .images {
    height: 300px;
}
}  
@media screen and (min-width: 768px) and (max-width: 991px) {
    .images {
    height: 350px;
}
}

</style>