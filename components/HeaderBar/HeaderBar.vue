<template>
  <div>
    <nav>
      <div class="container">
        <input id="nav-toggle" type="checkbox" />
        <div class="logo">
          <div class="spaceimg"></div>
          <h1 class="textHeader">วัดกันทรอมน้อย</h1>
        </div>
        <ul class="links">
          <li class="content-link">
            <NuxtLink to="/"><h3>หน้าแรก</h3></NuxtLink>
          </li>
          <li class="content-link">
            <NuxtLink to="/derivation"><h3>เกี่ยวกับ</h3></NuxtLink>
          </li>
          <li class="content-link">
            <NuxtLink to="/activity"><h3>กิจกรรม</h3></NuxtLink>
          </li>
          <li class="content-link">
            <NuxtLink to="/contact"><h3>ช่องทางติดต่อ</h3></NuxtLink>
          </li>
        </ul>
        <div></div>
      </div>
    </nav>
    <!-- media -->

    <div class="media">
      <v-app>
        <v-app-bar color="#FFECB3" class="flex-grow-0" app dark height="70">
          <v-app-bar-nav-icon
            v-click-outside="onClickOutside"
            @click="drawer = true"
          ></v-app-bar-nav-icon>
          <div class="itemhead">
            <div>
              <div class="itemcenter">
                <img class="logo" src="@/static/icons/logo.jpeg" alt="" />
                <h1>วัดกันทรอมน้อย</h1>
              </div>
            </div>
          </div>
        </v-app-bar>
        <div class="listmenu">
          <v-navigation-drawer app v-model="drawer" width="80%" color="#FFECB3">
            <v-list dense nav>
              <div class="sidemenu">
                <NuxtLink to="/">
                  <h3>หน้าแรก</h3>
                </NuxtLink>
                <NuxtLink to="/derivation">
                  <h3>เกี่ยวกับ</h3>
                </NuxtLink>
                <NuxtLink to="/activity">
                  <h3>กิจกรรม</h3>
                </NuxtLink>
                <NuxtLink to="/contact">
                  <h3>ช่องทางติดต่อ</h3>
                </NuxtLink>
              </div>
            </v-list>
          </v-navigation-drawer>
        </div>
      </v-app>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderBar',
  data: () => ({
    drawer: false,
  }),
}
</script>

<style lang="scss" scoped>
h3 {
  font-weight: bold;
  font-size: 1.25rem;
}
h3:hover {
  color: #ffb300;
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

.media {
  display: none;
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
@media screen and (min-width: 768px) and (max-width: 991px) {
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

@media screen and (max-width: 599px) {
  .media {
    display: block;
    width: 100%;
  }
  .container {
    display: none;
  }

  .sidemenu {
    margin-top: 10px;
    padding: 12px;
    padding-bottom: 0;
  }
  h3 {
    color: #000;
    text-align: left;
    font-size: 1.1rem;
    font-weight: 500;
    margin-bottom: 20px;
    padding-bottom: 10px;
  }
  h3:hover {
    color: #ffb300;
  }

  h2 {
    font-size: 1.25rem;
    font-weight: 500;
  }

  .listmenu {
    position: relative;
  }

  .v-application a {
    text-decoration: none;
  }
  .logo {
    border-radius: 30px;
    max-width: 50px;
    margin-left: 30px;
  }
  .itemcenter {
    display: flex;
    flex-direction: row;
    align-items: center;
  }
  h1 {
    color: #ffb300;
    margin-left: 30px;
  }
}
</style>
