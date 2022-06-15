<template>
  <div class="container">
    <div class="header">
        <h1>คติธรรมในการดำเนินชีวิต</h1>
    </div>

    <div class="contentImage">
        <v-row>
            <v-col cols="12" md="6">
                <img class="images" src="@/static/tamma1.png" alt="">
            </v-col>
            <v-col cols="12" md="6">
                <img class="images" src="@/static/tamma2.png" alt="">
            </v-col>
        </v-row>

        <v-row class="mt-8">
            <v-col cols="12" md="6">
                <img class="images" src="@/static/tamma3.png" alt="">
            </v-col>
            <v-col cols="12" md="6">
                <img class="images" src="@/static/tamma4.png" alt="">
            </v-col>
        </v-row>

        <v-row class="mt-8">
            <v-col cols="12" md="6">
                <img class="images" src="@/static/tamma5.png" alt="">
            </v-col>
            <v-col cols="12" md="6">
                <img class="images" src="@/static/tamma6.png" alt="">
            </v-col>
        </v-row>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Morale',
}
</script>

<style lang="scss" scoped>
.container {
  padding: 0;
  margin: 0;
  max-width: 100%;
  margin-top: 100px;
}
.header {
  display: flex;
  justify-content: center;
}
h1 {
  font-size: 3rem;
  color: #ff8f00;
  text-align: center;
  text-shadow: 2px 2px #fff;
  background-image: url("@/static/backgroung1.jpg");
  border-radius: 50px;
  padding-left: 50px;
  padding-right: 50px;
 
}
.contentImage {
    margin-top: 50px;
    display: flex;
    flex-direction: column;
    align-items: center;
    
}

.images {
    width: 100%;
    max-width: 600px;
   padding: 50px;
   padding-top: 0;
   padding-bottom: 0;
   height: auto;
   
}
@media screen and (max-width: 599px) {
  .container {
    margin-top: 50px;
  }
  h1 {
    font-size: 2rem;
  }
}
</style>
