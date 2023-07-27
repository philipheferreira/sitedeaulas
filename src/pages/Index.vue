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
    <div class="q-pa-lg">
      <q-table title="Disponibilidade de Horario" :rows="rows" :columns="columns" row-key="name" hide-bottom />
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

const columns = [
  {

    required: true,
    label: 'Segunda-Feira',
    align: 'center',
    field: (row) => row.name,
    format: (val) => `${val}`,
    sortable: true,
  },
  {
    name: 'Terça-feira', label: 'Terça-feira', field: 'fat', sortable: true,
  },
  { name: 'Quarta-feira', label: 'Quarta-feira', field: 'carbs' },
  { name: 'Quinta-feira', label: 'Quinta-feira', field: 'protein' },
  { name: 'Sexta-feira', label: 'Sexta-feira', field: 'sodium' },
  {
    name: 'Sabado', label: 'Sabado', field: 'calcium', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10),
  },
  {
    name: 'Domingo', label: 'Domingo', field: 'iron', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10),
  },
];

const rows = [
  {
    name: '14:00-15:00',
    fat: '14:00-15:00',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
  {
    name: '15:00-16:00',
    fat: '15:00-16:00',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
  {
    name: '-',
    fat: '16:00-17:00',
    carbs: '-',
    protein: '-',
    sodium: '16:00-17:00',
    calcium: '-',
    iron: '-',
  },
  {
    name: '-',
    fat: '-',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
  {
    name: '-',
    fat: '-',
    carbs: '-',
    protein: '-',
    sodium: '-',
    calcium: '-',
    iron: '-',
  },
];

export default defineComponent({
  name: "PageIndex",
  setup() {
    return {
      columns,
      rows
    }
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
