<template>
  <div class="container">
    <div class="headerText">
      <h1>วิดีโอแนะนำวัดกันทรอมน้อย</h1>
    </div>
    <div class="video">
      <iframe
        width="1000"
        height="500"
        src="https://www.youtube.com/embed/n16ITyG6-HA"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'P2Video',
}
</script>

<style lang="scss" scoped>
.container {
    background-image: url("@/static/backdround.jpg");
    margin: 0;
    padding: 0;
    max-width: 100%;
    height: 700px;
}
.headerText {
  margin-top: 30px;
}
h1 {
    padding-top: 30px;
    padding-bottom: 30px;
  font-size: 2.5rem;
  text-align: center;
  color: #000;
  text-shadow: 1px 1px #fff;
}
.video {
  display: flex;
  justify-content: center;
}
@media screen and (max-width: 599px) {
  .container {
    height: 300px;
  }
  h1 {
    font-size: 1.5rem;
  }
  iframe {
    width: 400px;
    height: auto;

  }
}
@media screen and (min-width: 768px) and (max-width: 991px)  {
    iframe {
    width: 500px;
    height: 400px;

  }
   .container {
    height: 600px;
  }
}
</style>
