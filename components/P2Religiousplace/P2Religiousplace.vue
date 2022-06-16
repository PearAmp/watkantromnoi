<template>
  <div class="container">
    <div class="headerText">
      <h1>เสนาสนะ ภายในวัดกันทรอมน้อย</h1>
    </div>
    <!-- item1 -->
    <div class="Itemcontent">
      <v-row class="item1">
        <v-col cols="6" class="borderRight">
          <img
            class="imageItems"
            src="https://pukmudmuangthai.com/wp-content/uploads/2021/02/Ao_izard-0122.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6">
          <div class="itemText">
            <h2>ศาลาการเปรียญ</h2>
            <p>ขนาดกว้าง ๑๖ เมตร ยาว ๒๙ เมตร</p>
            <p>สร้างเมื่อปี พ.ศ. ๒๕๓๕</p>
          </div>
        </v-col>
      </v-row>
    </div>

    <!-- item2 -->
    <div class="Itemcontent">
      <v-row class="item1">
        <v-col cols="6" class="borderRight">
          <img
            class="imageItems"
            src="https://pukmudmuangthai.com/wp-content/uploads/2021/02/Ao_izard-0122.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6">
          <div class="itemText">
            <h2>กุฏิเจ้าอาวาส</h2>
            <p>ขนาดกว้าง ๑๒ เมตร ยาว ๑๖ เมตร</p>
            <p>สร้างเมื่อปี พ.ศ. ๒๕๕๘</p>
          </div>
        </v-col>
      </v-row>
    </div>

    <!-- item3 -->
    <div class="Itemcontent">
      <v-row class="item1">
        <v-col cols="6" class="borderRight">
          <img
            class="imageItems"
            src="https://pukmudmuangthai.com/wp-content/uploads/2021/02/Ao_izard-0122.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6">
          <div class="itemText">
            <h2>กุฏิกัฏฐาน</h2>
            <p>จำนวน ๖ หลัง</p>
            <p>ขนาดกว้าง ๔ เมตร ยาว ๖ เมตร</p>
            <p>สร้างเมื่อปี พ.ศ. ๒๕๖๐</p>
          </div>
        </v-col>
      </v-row>
    </div>

    <!-- item4 -->
    <div class="Itemcontent">
      <v-row class="item1">
        <v-col cols="6" class="borderRight">
          <img
            class="imageItems"
            src="https://pukmudmuangthai.com/wp-content/uploads/2021/02/Ao_izard-0122.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6">
          <div class="itemText">
            <h2>กุฏิรับรอง</h2>
            <p>ขนาดกว้าง ๘ เมตร ยาว ๑๒ เมตร</p>
            <p>สร้างเมื่อปี พ.ศ. ๒๕๖๓</p>
          </div>
        </v-col>
      </v-row>
    </div>

    <!-- item5 -->
    <div class="Itemcontent">
      <v-row class="item1">
        <v-col cols="6" class="borderRight">
          <img
            class="imageItems"
            src="https://pukmudmuangthai.com/wp-content/uploads/2021/02/Ao_izard-0122.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6">
          <div class="itemText">
            <h2>อุโบสถ</h2>
            <p>ขนาดกว้าง ๓๐ เมตร ยาว ๕๐ เมตร</p>
            <p>สร้างเมื่อปี พ.ศ. ๒๕๕๙</p>
            <p>
              ทรงไทย ๒ ชั้น
              ช่อฟ้ารูปหงส์ ภายในปูด้วยหินแกรนิต
              ผนังวาดรูปเกี่ยวกับพุทธศาสนา
              ประตูและหน้าต่างทำด้วยไม้ตะเคียนแผ่นใหญ่ ชั้นล่างของโบสถ
              ปูด้วยหินแกรนิต ใช้สำหรับปฏิบัติธรรม ปัจจุบันสร็จสมบูรณ์แล้ว
            </p>
          </div>
        </v-col>
      </v-row>
    </div>

     <!-- item6 -->
    <div class="Itemcontent">
      <v-row class="item1">
        <v-col cols="6" class="borderRight">
          <img
            class="imageItems"
            src="https://pukmudmuangthai.com/wp-content/uploads/2021/02/Ao_izard-0122.jpg"
            alt=""
          />
        </v-col>
        <v-col cols="6">
          <div class="itemText">
            <h2>โรงครัว</h2>
            <p>ขนาดกว้าง ๘ เมตร ยาว ๑๖ เมตร</p>
            <p>สร้างเมื่อปี พ.ศ. ๒๕๕๖</p>
          </div>
        </v-col>
      </v-row>
    </div>


  </div>
</template>

<script>
export default {
  name: 'P2Religiousplace',
}
</script>

<style lang="scss" scoped>
.container {
  max-width: 1320px;
  height: auto;
  padding: 30px;
}
.headerText {
  margin-top: 30px;
}
h1 {
  font-size: 2.5rem;
  text-align: center;
  color: #ff8f00;
  text-shadow: 1px 1px #000;
}
.Itemcontent {
  margin-top: 40px;
  margin-bottom: 80px;
}
.item1 {
  height: auto;
  border: 2px solid #ff8f00;
  border-radius: 30px;
  display: flex;
  align-items: center;
}

.imageItems {
  width: 100%;
  max-width: 600px;
  height: 300px;
  padding: 20px;
  border-radius: 50px;
}
.borderRight {
  border-right: 2px solid #ff8f00;
}
.itemText {
  padding-left: 50px;
}
h2 {
  padding-bottom: 20px;
   color: #ff8f00;
}
p {
  padding: 10px;
}
@media screen and (max-width: 599px) {
    .headerText {
  margin-top: 0;
}

    
    h1 {
        font-size: 2rem;
    }

    .imageItems {
        max-width: 250px;
        height: 200px;
        padding: 0;
        border-radius: 30px;
    }
    h2 {
        font-size: 1.25rem;
        padding-bottom: 0;
       
    }
    p {
        padding: 0;
        font-size: 0.85rem;
    }
    .itemText {
  padding-left: 0;
}
}
@media screen and (min-width: 768px) and (max-width: 991px) {
.itemText {
  padding-left: 10px;
}
 .headerText {
  margin-top: 0;
}
    
}
</style>
