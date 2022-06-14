<template>
    <nav>
      <div class="container">
        <input id="nav-toggle" type="checkbox" />
        <div class="logo">
          <img class="imageIcon" src="https://scontent.fubp1-1.fna.fbcdn.net/v/t1.6435-9/31945732_1717066051663720_2583667676039610368_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=174925&_nc_eui2=AeErRaY9N8x7IZH-aoqMeZ7Onnm41PT3bQ-eebjU9PdtD6hjeUuOl7LoYhjXkiaMcLYB96UlpLMRRVg7DBtzrfRm&_nc_ohc=tEnQfiR_PjMAX_Cju8C&tn=_z4ScRnQjdZUWaSL&_nc_ht=scontent.fubp1-1.fna&oh=00_AT-6aJsTvKRVcSIjUNVgHXjd0XK5pzlT3213KuryR_ZkUw&oe=62CDFD60" />
           <div class="spaceimg"></div>
          <h1 class="textHeader">วัดกันทรอมน้อย</h1>
        </div>
        <ul class="links">
          <li class="content-link"><NuxtLink to="/"><h3>หน้าแรก</h3></NuxtLink></li>
          <li class="content-link">
            <NuxtLink to="/local"><h3>ความเป็นมา</h3></NuxtLink>
          </li>
          <li class="content-link"><NuxtLink to="/vaccines"><h3>กิจกรรม</h3></NuxtLink></li>
          <li class="content-link"><NuxtLink to="/contact"><h3>ช่องทางติดต่อ</h3></NuxtLink></li>
        </ul>
        <div>
          <div class="burger-icon">
            <ul>
              <label for="nav-toggle" class="icon-burger">
                <div class="line"></div>
                <div class="line"></div>
                <div class="line"></div>
              </label>
            </ul>
          </div>
        </div>
      </div>
    </nav>
</template>

<script>
export default {
    name: 'HeaderBar',

}
</script>

<style lang="scss" scoped>
.container {
  max-width: 100%;
  position: inherit;
  z-index: 10;
  left: 0;
  right: 0;
  top: 0;
  font-family: 'Monserrat', sans-serif;
  padding: 0.5%;
  height: 100px;
  background-color: #FFF8E1;

}

h3 {
  font-weight: 400;
}
h3:hover {
  color: #FFB300;

}

.imgicon {
  width: 30px;
  height: 30px;
}

nav .logo {
  float: left;
  width: 40%;
  height: 100%;
  display: flex;
  align-items: center;
  font-size: 24px;
  color: #000;
  flex-direction: row;
}
nav .links {
  margin: 0;
  width: 60%;
  height: 100%;
  display: flex;
  justify-content: space-around;
  padding-top: 30px;
}
.spaceimg {
    margin-right: 30px;
}
nav .links li {
  list-style: none;

}
nav .links a {
  display: block;
  padding: 1em;
  font-size: 16px;
  font-weight: bold;
  text-decoration: none;
  color: #000;

}
.imageIcon {
    width: 100%;
    max-width: 100px;
    height: 80px;
    border-radius: 50px;
}
.content-link {
  padding-top: 15px;
  
}

.burger-icon {
  display: none;
}
#nav-toggle {
  top: -100px;
  display: none;
}
.nav .icon-burger {
  display: none;
  top: 50%;
}
nav .icon-burger .line {
  width: 30px;
  height: 5px;
  background-color: #000;
  margin: 5px;
  border-radius: 3px;
  transition: all 0.3s ease-in-out;
}
@media screen and (max-width: 576px) {
  nav .logo {
    width: 75%;
    justify-content: center;
    padding-top: 10px;
    margin-left: 40px;
  }

  .imgicon {
    width: 40px;
    height: 40px;
  }

  .burger-icon {
    display: block;
    position: absolute;
    top: 2rem;
    right: 10px;
  }
  nav .links {
    float: none;
    position: fixed;
    z-index: 9;
    left: 0;
    right: 0;
    bottom: 100%;
    width: auto;
    height: 91%;
    flex-direction: column;
    justify-content: space-evenly;
    color: #fff;
    background-color: #fff;
    overflow: hidden;
    transition: all 0.5s ease-in-out;
  }
  nav .links a {
    font-size: 20px;
  }
  nav :checked ~ .links {
    bottom: 0;
  }
  nav .icon-burger {
    display: block;
  }
  nav :checked ~ .icon-burger .line:nth-child(1) {
    transform: translate(10px) rotate(225deg);
  }
  nav :checked ~ .icon-burger .line:nth-child(3) {
    transform: translate(10px) rotate(-225deg);
  }
  nav :checked ~ .icon-burger .line:nth-child(2) {
    opacity: 0;
  }
}
@media screen and (max-width: 599px) {
  h1 {
    font-size: 1.5rem;
  }
  .imageIcon {
    max-width: 60px;
    height: auto;
  }
  .spaceimg {
    margin-right: 10px;
  }
  
}
@media screen and (min-width: 768px) and (max-width: 991px)  {
  h1 {
    font-size: 1.5rem;
  } 
  nav .links a {
  display: block;
  padding: 0;
  padding-top: 25px;
  font-size: 0.9rem;

}

    
}
@media screen and (max-width: 1024px) {
  h1 {
    font-size: 1.5rem;
  } 
  nav .links a {
  display: block;
  padding: 0;
  padding-top: 25px;
  font-size: 0.9rem;

}
}
</style>
