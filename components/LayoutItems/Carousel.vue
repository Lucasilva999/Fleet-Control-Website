<template>
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
</template>

<script>
export default {
    
}
</script>