<template>
  <v-layout row ma-2>
    <v-flex xs12 class="mb-extra">
      <h2 class="title text-center">CONECTANDO O VEÍCULO AO SEU NEGÓCIO</h2>
      <p class="subtitle-1 text-center">
        VOCÊ NÃO PRECISA TER UM GERENTE DE FROTAS PARA UTILIZAR NOSSO SISTEMA. SIMPLES DE USAR, ALTA TECNOLOGIA PARA FROTAS PEQUENAS ATRAVÉS DE UM CONJUNTO COMPLETO DE PRODUTOS PARA RASTREAMENTO VEICULAR, GESTÃO DE FROTAS, ROTEIRIZAÇÃO E GERENCIAMENTO DE ENTREGAS E SERVIÇOS: TUDO INTEGRADO EM UMA ÚNICA PLATAFORMA.
      </p>
    </v-flex>
    <v-flex xs12 class="mb-extra" color="indigo" lighten-4>
          <v-row>
             <v-col cols=3 class="d-flex justify-center">
              <v-card>
                <v-avatar size="125px">
                  <v-img contain src="avatars/1.jpg"></v-img>
                </v-avatar>
                <v-card-text>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore temporibus et quas velit consequatur atque natus voluptatum eius est rem unde!</p>
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols=3 class="d-flex justify-center">
              <v-card>
                <v-avatar size="125px">
                  <v-img contain src="avatars/2.jpg"></v-img>
                </v-avatar>
                <v-card-text>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore temporibus et quas velit consequatur atque natus voluptatum eius est rem unde!</p>
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols=3 class="d-flex justify-center">
              <v-card>
                <v-avatar size="125px">
                  <v-img contain src="avatars/3.jpg"></v-img>
                </v-avatar>
                <v-card-text>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore temporibus et quas velit consequatur atque natus voluptatum eius est rem unde!</p>
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols=3 class="d-flex justify-center">
              <v-card>
                <v-avatar size="125px">
                  <v-img contain src="avatars/4.jpg"></v-img>
                </v-avatar>
                <v-card-text>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore temporibus et quas velit consequatur atque natus voluptatum eius est rem unde!</p>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
    </v-flex>
    <IMG source="/1.jpg" class="mb-extra"/>
    <Topico class="pl-5"/>
    <IMG source="/2.jpg" class="mb-extra"/>
    <Topico class="pl-5"/>
    <IMG source="/3.jpg" class="mb-extra"/>
    <Topico class="pl-5 mb-extra"/>
    <v-flex xs12 class="mb-5">
      <h2 class="title text-center">PORQUE USAR NOSSO CONTROLE DE FROTAS?</h2>
      <p class="subtitle-1 text-center">REPLETO DE RECURSOS, DESEMPENHO PARA SEU VEÍCULO TRABALHAR COMO NUNCA!</p>
    </v-flex>
    <v-flex xs12 md4 class="pa-5">
      <v-img contain position="center center" src="/icons/gas.png" height="100px"></v-img>
      <p class="my-4 text-center title">Controle de Combustível</p>
      <p class="text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus vel maiores aperiam excepturi eveniet modi quod minima quaerat, in accusantium et, omnis autem?</p>
    </v-flex>
    <v-flex xs12 md4 class="pa-5">
      <v-img contain position="center center" src="/icons/map.png" height="100px"></v-img>
      <p class="my-4 text-center title">Localização em Tempo Real</p>
      <p class="text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus vel maiores aperiam excepturi eveniet modi quod minima quaerat, in accusantium et, omnis autem?</p>
    </v-flex>
    <v-flex xs12 md4 class="pa-5">
      <v-img contain position="center center" src="/icons/money-bag.png" height="100px"></v-img>
      <p class="my-4 text-center title">Redução de Gastos</p>
      <p class="text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus vel maiores aperiam excepturi eveniet modi quod minima quaerat, in accusantium et, omnis autem?</p>
    </v-flex>
    <v-flex xs12 class="text-center">
      <v-btn dark color="indigo" class="text-center mb-extra">Solicite um Contato</v-btn>
    </v-flex>
    
    
    
  </v-layout>
</template>

<script>
import IMG from '@/components/ImagensHome.vue';
import Topico from '@/components/TopicosHome.vue';

export default {
  components: {
    IMG, Topico
  }
}
</script>

<style scoped>
  .mb-extra {
    margin-bottom: 75px;
  }

</style>
