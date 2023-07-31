<template>
  <div class="q-pa-lg">
    <q-table title="Disponibilidade de Horario" :rows="rows" :columns="columns" row-key="name" hide-bottom />
  </div>
</template>

<script>

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


export default {
  setup() {
    return {
      columns,
      rows
    }
  }
}
</script>

<style></style>
