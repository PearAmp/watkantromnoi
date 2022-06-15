<template>
<div class="container">
    <div class="header">
        <h1>พระอธิการ และพระลูกวัด</h1>
    </div>

    <div class="mt-10">
        <v-window
      v-model="onboarding"
      reverse
    >
      <v-window-item
        v-for="n in length"
        :key="`card-${n}`"
      >
        <v-card
          color="#FFECB3"
          height="400"
        >
          <v-row
            class="fill-height"
            justify="center"
          >
            <img class="imageBudda" src="@/static/budda.jpeg" alt="" />
             <img class="imageBudda" src="@/static/budda.jpeg" alt="" />
              <img class="imageBudda" src="@/static/budda.jpeg" alt="" />
              <img class="imageBudda" src="@/static/budda.jpeg" alt="" />
              <img class="imageBudda" src="@/static/budda.jpeg" alt="" />
             
          </v-row>
        </v-card>
      </v-window-item>
    </v-window>

    <v-card-actions class="justify-space-between">
      <v-btn
        text
        @click="prev"
      >
        <v-icon>mdi-chevron-left</v-icon>
      </v-btn>
      <v-item-group
        v-model="onboarding"
        class="text-center"
        mandatory
      >
        <v-item
          v-for="n in length"
          :key="`btn-${n}`"
          v-slot="{ active, toggle }"
        >
          <v-btn
            :input-value="active"
            icon
            @click="toggle"
          >
            <v-icon>mdi-record</v-icon>
          </v-btn>
        </v-item>
      </v-item-group>
      <v-btn
        text
        @click="next"
      >
        <v-icon>mdi-chevron-right</v-icon>
      </v-btn>
    </v-card-actions>
    </div>
</div>
  
</template>

<script>
export default {
    name: 'Personal',

    data: () => ({
      length: 3,
      onboarding: 0,
    }),

    methods: {
      next () {
        this.onboarding = this.onboarding + 1 === this.length
          ? 0
          : this.onboarding + 1
      },
      prev () {
        this.onboarding = this.onboarding - 1 < 0
          ? this.length - 1
          : this.onboarding - 1
      },
    },

}
</script>

<style lang="scss" scoped>
.container {
    margin-top: 100px;
    padding: 0;
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
.imageBudda {
    width: 200px;
    height: auto;
    margin: 50px;
    border-radius: 30px;
}
@media screen and (max-width: 599px) {
    .container {
        margin-top: 50px;
        padding: 12px;
    }
    h1 {
        font-size: 1.7rem;
    }
    
}
</style>