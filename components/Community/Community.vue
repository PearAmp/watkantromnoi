<template>
  <div class="container">
    <div class="header">
      <h1>วัด และ ชุมชน</h1>
    </div>

    <!-- activity -->
    <div class="content">
      <v-row>
        <v-col cols="12" md="4" sm="4">
          <img class="Imagecontent" src="@/static/watktncovid.jpeg" alt="" />
          <div class="textcontent">
            <h3>กิจกรรมมอบถุงยังชีพและอาหาร</h3>
            <p>ให้กับญาติโยมชาวบ้านกันทรอมน้อยและบ้านไทรน้อย</p>
            <p>จำนวน 170 ครัวเรือน</p>
          </div>
        </v-col>
        <v-col cols="12" md="4" sm="4">
          <img class="Imagecontent" src="@/static/watktnhumen2.jpeg" alt="" />
          <div class="textcontent">
            <h3>เทพื้นคอนกรีต รอบอุโบสถ</h3>
            <p>ขอ อนุโมทนากับญาติโยมทั้งสองหมู่บ้านที่ช่วย</p>
            <p>เทพื้นคอนกรีต รอบอุโบสถในวันนี้</p>
          </div>
        </v-col>
        <v-col cols="12" md="4" sm="4">
          <img class="Imagecontent" src="@/static/watktnhumen.jpeg" alt="" />
          <div class="textcontent">
            <h3>งานฉลองอุโบสถวัดกันทรอมน้อย</h3>
            <p>ร่วมด้วยผู้นำชุมชน และลูกบ้าน ทั้งบ้านกันทรอมน้อย</p>
            <p>ไทรน้อย ช่วยกันเตรียมงาน และจัดสถานที่</p>
          </div>
        </v-col>
      </v-row>

      <!-- activity 2 -->
      <v-row>
        <v-col cols="12" md="4" sm="4">
          <img class="Imagecontent" src="@/static/watktnhumen6.jpeg" alt="" />
          <div class="textcontent">
            <h3>ศาลาการเปรียญ</h3>
            <p>ชาวบ้านกันทรอมน้อย ร่วมใจ สร้างศาลาการเปรียญ</p>
            <p>หลังใหม่ เพื่อใช้ในการประชุม หรือใช้ประโยชน์อื่น</p>
          </div>
        </v-col>
        <v-col cols="12" md="4" sm="4">
          <img class="Imagecontent" src="@/static/watktnhumen4.jpeg" alt="" />
          <div class="textcontent">
            <h3>ขอเชิญร่วมบุญ</h3>
            <p>พิธีผูกพัทธสีมาปิดทองตัดหวายลูกนิมิตอุโบสถ</p>
            <p>ระหว่างวันที่ ๑ - ๕ กุมภาพันธ์ พ.ศ. ๒๕๖๕</p>
          </div>
        </v-col>
        <v-col cols="12" md="4" sm="4">
          <img class="Imagecontent" src="@/static/watktnhumen5.jpeg" alt="" />
          <div class="textcontent">
            <h3>ทำความสะอาดวัดในวันออกพรรษา</h3>
            <p>ร่วมด้วยผู้นำชุมชน และลูกบ้าน ทั้งบ้านกันทรอมน้อย</p>
            <p>ไทรน้อย ช่วยกันทำความสะอาดบริเวณวัด</p>
          </div>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Community',
}
</script>

<style lang="scss" scoped>
.container {
  max-width: 100%;
  height: auto;
  
}
.header {
  display: flex;
  justify-content: center;
}
h1 {
  margin-top: 100px;
  font-size: 3rem;
  color: #ff8f00;
  text-align: center;
  background-image: url("@/static/backgroung1.jpg");
  border-radius: 50px;
  padding-left: 50px;
  padding-right: 50px;
  text-shadow: 2px 2px #fff;
}

.Imagecontent {
  width: 100%;
  max-width: 500px;
  height: 300px;
  padding: 50px;
  padding-bottom: 0;
 
}
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.textcontent {
  padding-top: 10px;
  text-align: center;
}
p {
  margin: 0;
  font-size: 18px;
}
h3 {
  padding-bottom: 10px;
}
@media screen and (max-width: 599px) {
  h1 {
    margin-top: 30px;
    font-size: 2rem;
  }
  .border {
    margin-left: 20%;
    margin-right: 20%;
  }
}
@media screen and (min-width: 768px) and (max-width: 991px) {
  h1 {
    margin-top: 30px;
    font-size: 2.5rem;
  }

  .border {
    margin-left: 35%;
    margin-right: 35%;
  }
}
@media screen and (max-width: 1420px) {
  h1 {
    margin-top: 30px;
    font-size: 2.5rem;
  }

  .border {
    margin-left: 35%;
    margin-right: 35%;
  }
}
</style>
