<template>
    <v-layout row class="ma-2">
        <IMG source="/1.jpg" class="mb-3"/>
        <Topico class="mb-5"/>
        <IMG source="/2.jpg" class="mb-3"/>
        <Topico class="mb-5"/>
        <IMG source="/3.jpg" class="mb-3"/>
        <Topico class="mb-5"/>
    </v-layout>
</template>

<script>
import IMG from '@/components/TopicosSection/Imagem.vue';
import Topico from '@/components/TopicosSection/Topico.vue';

export default {
    components: { IMG, Topico }
}
</script>


<style scoped>
  .mb-extra {
    margin-bottom: 75px;
  }

</style>