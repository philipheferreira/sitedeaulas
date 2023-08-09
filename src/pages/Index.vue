<template>
  <q-page>
    <div class="info q-ma-lg">
      <h5 class="text-center">Professor Milton Oliveira</h5>
      <div class="row items-center">
        <img class="col-6 q-ma-sm" alt="Quasar logo" src="../img/FotoMilton.jpeg" style="height: 250px; width: 200px;" />
        <p class="texto col">Estudo a um tempo como a matemática afeta a aprendizagem e sua importância dentro do estudo
          geral
          humano.
          Trabalho com meus alunos dentro da perspectiva de auxiliá-los no contato com a disciplina e aprimoramento
          pessoal.<br />
          <strong>Formação:</strong> Licenciatura plena em matemática na UFPA em 2019
        </p>
      </div>
      <timeline></timeline>
      <p>informações</p> <!-- as infos da pagina está funcionando com base de uma gambiarra -->
    </div>
    <tabelaHorarios></tabelaHorarios>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import tabelaHorarios from "components/TabelaHorarios.vue";
import timeline from "components/TimeLine.vue";

export default defineComponent({
  name: "PageIndex",
  components: {
    tabelaHorarios,
    timeline
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
