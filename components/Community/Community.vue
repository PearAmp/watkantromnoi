<template>
  <div class="container">
    <div class="header">
        <h1 class="textHead">วัด และ ชุมชน</h1>
    </div>
    
  </div>
</template>

<script>
export default {
    name: 'Community',

}
</script>

<style lang="scss" scoped>
.header {
    display: flex;
    justify-content: center
}
.textHead {
    margin-top: 100px;
    font-size: 3rem;
    color: #FF8F00;
     border-bottom: 3px solid #FF8F00;
    width: 20%;
    display: flex;
    justify-content: center;
}
@media screen and (max-width: 599px) {
    .textHead {
         width: 100%;
         margin-top: 30px;
         font-size: 2.5rem;
    }
    
}
@media screen and (min-width: 768px) and (max-width: 991px) {
    .textHead {
         width: 50%;
         margin-top: 30px;
         font-size: 2.5rem;
    }
}
@media screen and (max-width: 1420px) {
     .textHead {
         width: 40%;
         margin-top: 30px;
         font-size: 2.5rem;
    }
    
}
</style>