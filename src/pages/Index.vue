<template>
  <q-page class="">
    <div class="info q-ma-lg">
      <h5 class="text-center">Professor Milton Oliveira</h5>
      <div class="column items-center">
        <img alt="Quasar logo" src="../img/FotoMilton.jpeg" style="height: 300px; width: 300px;" class="q-ma-md" />
      </div>
      <p class="texto">Estudo a um tempo como a matemática afeta a aprendizagem e sua importância dentro do estudo geral
        humano.
        Trabalho com meus alunos dentro da perspectiva de auxiliá-los no contato com a disciplina e aprimoramento pessoal
      </p>
      <p class="texto"><strong>Formação:</strong> Licenciatura plena em matemática na UFPA em 2019</p>
    </div>
    <tabelaHorarios></tabelaHorarios>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import tabelaHorarios from "components/TabelaHorarios.vue"

export default defineComponent({
  name: "PageIndex",
  components: {
    tabelaHorarios
  }
});
</script>

<style>
body {
  background-color: #FFFFFF;
}

.info {
  padding: 0px 20px;
  background-color: #f5f5f5;
  border-radius: 15px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
}

.texto {
  color: #5c5c5c;
}
</style>
