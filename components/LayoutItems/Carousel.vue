<template>
<v-carousel
    cycle 
    hide-delimiters
    hide-delimiter-background
    show-arrows-on-hover
>
    <v-carousel-item
      v-for="(color, i) in colors"
      :key="color"
    >
      <v-sheet
        :color="color"
        height="100%"
        tile
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="display-3">Slide {{ i + 1 }}</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
    data () {
      return {
        colors: [
          'primary',
          'secondary',
          'yellow darken-2',
          'red',
          'orange',
        ],
      }
    },
  }
</script>

<!--
  <v-carousel
        hide-delimiters
        cycle
        height="400"
        hide-delimiter-background
        show-arrows-on-hover
      >
        <v-carousel-item>
            <v-row
              class="fill-height"
              align="center"
              justify="center"
            >
              <v-img src="slider/1.jpg" position="center center"></v-img>
            </v-row>
        </v-carousel-item>
        <v-carousel-item>
            <v-row
              class="fill-height"
              align="center"
              justify="center"
            >
              <v-img src="slider/2.jpg"></v-img>
            </v-row>
        </v-carousel-item>
        <v-carousel-item>
            <v-row
              class="fill-height"
              align="center"
              justify="center"
            >
              <v-img src="slider/3.jpg"></v-img>
            </v-row>
        </v-carousel-item>
      </v-carousel>
  -->