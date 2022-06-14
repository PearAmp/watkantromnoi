<template>
       <div>
          <v-carousel class="Onweb" hide-delimiters height="700" cycle show-arrows-on-hover="false" show-arrows="false" >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
  <!-- notebook -->
  <v-carousel class="notebook" hide-delimiters height="500" cycle show-arrows-on-hover="false" show-arrows="false" >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
  <!-- ipad -->
  <v-carousel class="Ipad" hide-delimiters height="500" cycle show-arrows-on-hover="false" show-arrows="false" >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>

       <!-- media -->
         <v-carousel class="Media" hide-delimiters height="300" cycle show-arrows-on-hover="false" show-arrows="false" >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
       </div>
</template>

<script>
export default {
    name: 'ImageHeader',
    data () {
      return {
        items: [
          {
            src: require('@/static/watktn.jpeg'),
          },
          {
            src: require('@/static/watktn2.jpeg'),
          },
          {
            src: require('@/static/watktn3.jpeg'),
          },
          {
            src: require('@/static/watktn4.jpeg'),
          },
        ],
      }
    },

}
</script>

<style lang="scss" scoped>
.Media {
  display: none;
}
.Ipad {
   display: none;
}
.notebook {
  display: none;
}
@media screen and (min-width: 768px) and (max-width: 991px) {
  .Ipad {
   display: block;
}
 .Media {
   display: none;
  }
  .Onweb {
    display: none;
  }
  .notebook {
  display: none;
}
}
@media screen and (max-width: 1024px) {
  .notebook {
  display: block;
}
 .Ipad {
   display: none;
}
 .Media {
   display: none;
  }
  .Onweb {
    display: none;
  }

}
@media screen and (max-width: 599px) {
  .Media {
   display: inline;
  }
  .Onweb {
    display: none;
  }
  .Ipad {
   display: none;
}
.notebook {
  display: none;
}
  
}

    
</style>