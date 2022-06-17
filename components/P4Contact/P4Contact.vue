<template>
  <div class="container">
    <div class="contact">
      <v-row>
        <v-col cols="4">
          <div class="box">
            <img class="imageIcons" src="@/static/icons/location.png" alt="" />
          </div>
          <div class="texttitle">
            <h1>ที่ตั้ง</h1>
            <p>
              ตั้งอยู่ที่บ้านกันทรอมน้อย หมู่ที่ ๖ ตำบลกันทรอม อำเภอขุนหาญ
              จังหวัดศรีสะเกษ
            </p>
          </div>
        </v-col>
        <v-col cols="4">
          <div class="box">
            <img class="imageIcons" src="@/static/icons/telephone.png" alt="" />
          </div>
          <div class="texttitle">
            <h1>หมายเลขติดต่อ</h1>
            <p><span>หมายเลขหลัก : </span>088 - 722 - 6256</p>
            <p><span>พระธงชัย : </span>091 - 874 - 8880</p>
          </div>
        </v-col>
        <v-col cols="4">
          <div class="box">
            <img class="imageIcons" src="@/static/icons/facebook.png" alt="" />
          </div>
          <div class="texttitle">
            <h1>เพจ</h1>

            <div class="pageContact">
              <img class="imagePage" src="@/static/icons/page.jpg" alt="" />
              <p class="textcontent">เพจวัดกันทรอมน้อย</p>
            </div>
          </div>
        </v-col>
      </v-row>
    </div>
    <!-- mobile -->
    <div class="Mobile">
      <v-row>
        <v-col cols="6" class="border">
          <div class="box">
            <img class="imageIcons" src="@/static/icons/location.png" alt="" />
          </div>
          <div class="media">
            <h1>ที่ตั้ง</h1>
          </div>
        </v-col>
        <v-col cols="6" class="centertext">
          <p>
            ตั้งอยู่ที่บ้านกันทรอมน้อย หมู่ที่ ๖ ตำบลกันทรอม อำเภอขุนหาญ
            จังหวัดศรีสะเกษ
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="6" class="border">
          <div class="box">
            <img class="imageIcons" src="@/static/icons/telephone.png" alt="" />
          </div>
          <div class="media">
            <h1>หมายเลขติดต่อ</h1>
          </div>
        </v-col>
        <v-col cols="6" class="centertext">
          <p>หมายเลขหลัก :</p>
          <p>088 - 722 - 6256</p>
          <p>พระธงชัย :</p>
          <p>091 - 874 - 8880</p>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="6" class="border">
          <div class="box">
            <img class="imageIcons" src="@/static/icons/facebook.png" alt="" />
          </div>
          <div class="media">
            <h1>เพจ</h1>
          </div>
        </v-col>
        <v-col cols="6" class="centertext">
          <img class="imagePage" src="@/static/icons/page.jpg" alt="" />
          <p class="textcontent">เพจวัดกันทรอมน้อย</p>
        </v-col>
      </v-row>
    </div>

    <!-- Map -->
    <div class="map">
      <div>
        <h1 class="textMap">วัดกันทรอมน้อย อำเภอขุนหาญ จังหวัดศรีสะเกษ</h1>
      </div>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d61795.63091761368!2d104.31879255919554!3d14.529008056532701!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31112ac888565e0b%3A0x31e036b9203ceea5!2z4Lin4Lix4LiU4Lia4LmJ4Liy4LiZ4LiB4Lix4LiZ4LiX4Lij4Lit4Lih4LiZ4LmJ4Lit4Lii!5e0!3m2!1sth!2sth!4v1655445458113!5m2!1sth!2sth"
        width="1000"
        height="500"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'P4Contact',
}
</script>

<style lang="scss" scoped>
.container {
  max-width: 100%;
  height: auto;
}
.contact {
  margin-top: 100px;
}
h1 {
  text-align: center;
  padding-top: 30px;
  color: #263238;
  text-shadow: 2px 2px #ffc400;
  font-size: 2.5rem;
}

p {
  margin-top: 20px;
  padding: 50px;
  padding-top: 0;
  font-size: 1.4rem;
  padding-bottom: 0;
}
.box {
  border: 2px solid #ffcc80;
  width: 100%;
  max-width: 120px;
  border-radius: 60px;
  display: flex;
  justify-content: center;
  padding: 20px;
}
.imageIcons {
  width: 100%;
  max-width: 100px;
  height: auto;
}
.col-4 {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.pageContact {
  display: flex;
  flex-direction: row;
  align-items: center;
}
.imagePage {
  width: 100%;
  max-width: 100px;
  height: auto;
  border-radius: 50px;
}
.textcontent {
  font-weight: bold;
  color: #ffc400;
  text-shadow: 1px 1px #ff6d00;
  font-size: 2rem;
}
.Mobile {
  display: none;
}
.map {
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 50px;
}
.textMap {
  color: #ff6d00;
  margin-bottom: 50px;
}

@media screen and (max-width: 1420px) {
  .Mobile {
    display: none;
  }
  .imageIcons {
    max-width: 60px;
  }
  .box {
    max-width: 100px;
    border-radius: 70px;

    padding: 20px;
  }
  .contact {
    margin-top: 50px;
  }
  h1 {
    font-size: 2rem;
  }
  p {
    font-size: 1rem;
    padding: 0;
  }
  .imagePage {
    max-width: 80px;
  }
  .textcontent {
    font-size: 1.5rem;
    padding-left: 20px;
  }
}
@media screen and (min-width: 768px) and (max-width: 991px) {
  .Mobile {
    display: none;
  }
  h1 {
    font-size: 1.8rem;
  }
  .pageContact {
    flex-direction: column;
    margin-top: 20px;
  }
  iframe {
    width: 700px;
    height: 400px;
  }
}
@media screen and (max-width: 599px) {
  .map {
    margin-top: 30px;
    padding: 20px;
    padding-top: 0;
  }
  .textMap {
    margin-bottom: 20px;
  }
  iframe {
    width: 400px;
    height: 250px;
  }
  .Mobile {
    display: block;
  }
  .contact {
    display: none;
  }
  .col-6 {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  h1 {
    padding-top: 10px;
    font-size: 1.5rem;
  }
  .imageIcons {
    max-width: 50px;
  }
  .box {
    border: none;
  }
  .border {
    border-right: 2px solid #ffcc80;
    margin-top: 20px;
  }
  .centertext {
    display: flex;
    justify-content: center;
  }
  p {
    font-size: 1rem;
  }
  .imagePage {
    margin-top: 20px;
    max-width: 100px;
  }
  .textcontent {
    font-size: 1.25rem;
    text-align: center;
  }
}
</style>
