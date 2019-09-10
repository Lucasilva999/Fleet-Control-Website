<template>  
    <v-flex xs12 md6>
      <v-img contain :src="source" max-height="340"></v-img>
    </v-flex>
</template>

<script>
export default {
    name: 'ImagensHome',
    props: {
        source: {
            type: String,
            required: true
        }
    }
}
</script>