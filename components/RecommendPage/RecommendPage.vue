<template>
  <div class="container">
    <v-row class="record">
      <v-col cols="12" md="6" class="tt" sm="6">
        <img class="imageLeft" src="@/static/watktn1.jpeg" />
      </v-col>
      <v-col class="textrigth" cols="12" md="6" sm="6">
        <h1>วัดกันทรอมน้อย</h1>
        <p class="textcontent">
          วัดกันทรอมน้อยสร้างเมื่อ พ.ศ. ๒๕๑๙ ตั้งอยู่ที่บ้านกันทรอมน้อย หมู่ที่
          ๖ ตำบลกันทรอม อำเภอขุนหาญ จังหวัดศรีสะเกษ มีเนื้อที่ ๑๒ ไร่ ๒๖ ตารางวา
          การสร้างวัดเริ่มจากการแลกที่ดินของ ครูไมตรี วงษ์นิล กับ พ่อเทพ สมรัตน์
          ครูไมตรี วงษ์นิล จึงได้มอบที่ดินให้สร้างวัดจำนวน ๑๒ ไร่ ๒๖ ตารางวา
          โดยเริ่มสร้างจากชาวบ้านกันทรอมน้อย นำโดย พ่อพรหม สมรัตน์ พ.ศ.
          ไม่ทราบแน่ชัด โดยบอกต่อกันมารุ่นสู่รุ่น และ พ.ศ. ๒๕๑๙ โดยมี หลวงพ่อเชน
          ฉายาไม่ทราบ (อดีตจ้าอาวาส) เป็นผู้ก่อตั้งวัดขึ้นมา
        </p>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'RecommendPage',
}
</script>

<style lang="scss" scoped>
.container {
  margin: 0;
  padding: 0;
}
.record {
  margin-top: 40px;
  padding-left: 80px;
}
.imageLeft {
  width: 100%;
  max-width: 1000px;
  height: auto;
  border-radius: 40px;
}
.textrigth {
  padding-left: 100px;
  align-self: center;
}
.textcontent {
    width: 85%;
    margin-top: 20px;
}

@media screen and (max-width: 599px) {
    .record {
        padding-left: 0;
        padding: 12px;
        margin-top: 10px;
    }
    .textrigth {
        padding-left: 50px;
    }
    h1 {
        text-align: center;
    }
    .textcontent {
    width: 90%;
}

    
}
@media screen and (min-width: 768px) and (max-width: 991px) {
     .record {
        padding-left: 0;
    }
    .textrigth {
        padding-left: 50px;
    }
    h1 {
        text-align: center;
    }
    .textcontent {
    width: 90%;
}
.imageLeft {
  height: 400px;
}
}
// .tt {
//   background-color: #000;
// }
</style>
