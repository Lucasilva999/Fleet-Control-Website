<template>
    <v-layout row>
        <IMG source="/1.jpg" class="mb-extra"/>
        <Topico class="pl-5"/>
        <Topico class="pl-5 mb-extra"/>
        <IMG source="/2.jpg" class="mb-extra"/>
        <IMG source="/3.jpg" class="mb-extra"/>
        <Topico class="pl-5 mb-extra"/>
    </v-layout>
</template>

<script>
import IMG from '@/components/ImagensHome.vue';
import Topico from '@/components/TopicosHome.vue';

export default {
    components: { IMG, Topico }
}
</script>


<style scoped>
  .mb-extra {
    margin-bottom: 75px;
  }

</style>