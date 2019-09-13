<template>
  <v-layout row>
    <v-flex xs12 class="mb-5">
      <h2 class="title text-center">CONECTANDO O VEÍCULO AO SEU NEGÓCIO</h2>
      <p class="subtitle-1 text-center">
        VOCÊ NÃO PRECISA TER UM GERENTE DE FROTAS PARA UTILIZAR NOSSO SISTEMA. SIMPLES DE USAR, ALTA TECNOLOGIA PARA FROTAS PEQUENAS ATRAVÉS DE UM CONJUNTO COMPLETO DE PRODUTOS PARA RASTREAMENTO VEICULAR, GESTÃO DE FROTAS, ROTEIRIZAÇÃO E GERENCIAMENTO DE ENTREGAS E SERVIÇOS: TUDO INTEGRADO EM UMA ÚNICA PLATAFORMA.
      </p>
    </v-flex>
    <TopSection/>
    
    <TopicosSection v-if="$vuetify.breakpoint.smAndUp"/>
    <TopicosSectionMobile v-if="$vuetify.breakpoint.xsOnly"/>
    
    <v-flex xs12 class="mb-5">
        <h2 class="title text-center">PORQUE USAR NOSSO CONTROLE DE FROTAS?</h2>
        <p class="subtitle-1 text-center">REPLETO DE RECURSOS, DESEMPENHO PARA SEU VEÍCULO TRABALHAR COMO NUNCA!</p>
    </v-flex>
    <BottomSection/>
    <v-flex xs12 class="text-center">
      <v-btn dark color="indigo" class="text-center mb-extra">Solicite um Contato</v-btn>
    </v-flex>

  </v-layout>
</template>

<script>
import TopSection from '@/components/TopSection/TopSection.vue';
import BottomSection from '@/components/BottomSection/BottomSection.vue';
import TopicosSection from '@/components/TopicosSection/TopicosSection.vue';
import TopicosSectionMobile from '@/components/TopicosSection/TopicosSectionMobile.vue';

export default {
  components: {
    TopSection, BottomSection, TopicosSection, TopicosSectionMobile
  }

}
</script>

<style scoped>
  .mb-extra {
    margin-bottom: 75px;
  }

</style>
