<template>
  <v-app>
    <Nav></Nav>
    <v-carousel height="800"
      hide-delimiter-background
      show-arrows="false">
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <v-sheet :color="colors[i]" height="100%">
          <v-row class="fill-height" align="center" justify="center">
            <div class="display-4" >{{ slide }} Slide</div>
          </v-row>
        </v-sheet>
      </v-carousel-item>
    </v-carousel>
    <Footer></Footer>
  </v-app>
</template>

<script>
import Nav from "./Nav";
import Footer from "./Footer";

export default {
  name: "Home",
  components: {
    Nav,
    Footer
  },
  data() {
    return {
      colors: [
        'indigo', 'warning', 'pink darken-2', 'red lighten-1', 'deep-purple accent-4'
      ],
      slides: [
        'First', 'Second', 'Third', 'Fourth', 'Fifth'
      ]
    };
  }
};
</script>

<style lang="stylus">
#example-custom-transition {
  .fade {
    &-enter-active, &-leave-active, &-leave-to {
      transition: 0.3s ease-out;
      position: absolute;
      top: 0;
      left: 0;
    }

    &-enter, &-leave, &-leave-to {
      opacity: 0;
    }
  }
}
</style>
