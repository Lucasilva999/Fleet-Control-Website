<template>
  <v-layout row>
    <v-flex xs12 class="mb-5">
      <h2 class="display-1 text-center mb-3">CONECTANDO O VEÍCULO AO SEU NEGÓCIO</h2>
      <p class="subtitle-1 text-center">
        VOCÊ NÃO PRECISA TER UM GERENTE DE FROTAS PARA UTILIZAR NOSSO SISTEMA. SIMPLES DE USAR, ALTA TECNOLOGIA PARA FROTAS PEQUENAS ATRAVÉS DE UM CONJUNTO COMPLETO DE PRODUTOS PARA RASTREAMENTO VEICULAR, GESTÃO DE FROTAS, ROTEIRIZAÇÃO E GERENCIAMENTO DE ENTREGAS E SERVIÇOS: TUDO INTEGRADO EM UMA ÚNICA PLATAFORMA.
      </p>
    </v-flex>
    <TopSection/>
    <v-flex xs12 class="mb-extra">
      <h2 class="headline text-center mb-3">CONTROLE PARA O VEÍCULO DESEMPENHAR SUAS ATIVIDADES</h2>
      <p class="subtitle-1 text-center">
        TENHA O CONTROLE DOS GASTOS DE CADA VEÍCULO, GERENCIE CUSTOS COMO ABASTECIMENTOS E MANUTENÇÕES. ORGANIZE SUA FROTA, GERENCIE MULTAS, PNEUS, MANUTENÇÕES PREVENTIVAS E CORRETIVAS. TODO O CONTROLE NECESSÁRIO PARA QUE UM VEÍCULO POSSA DESEMPENHAR SUAS FUNÇÕES VOCÊ PODE GERENCIAR ATRAVÉS DO MÓDULO DE GESTÃO DE FROTAS DO ROTAEXATA.
      </p>
    </v-flex>
    <TopicosSection v-if="$vuetify.breakpoint.mdAndUp"/>
    <TopicosSectionMobile v-else/>
    
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
