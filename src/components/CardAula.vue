<template>
  <q-card class="my-card q-ma-md">
    <q-video :src=site />

    <q-card-section>
      <div class="text-h6"> {{ titulo }} </div>
      <div class="text-subtitle2">{{ autor }}</div>
    </q-card-section>

    <q-card-section class="q-pt-none">
      {{ sobre }}
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  props: ['site', 'titulo', 'autor', 'sobre']
}
</script>

<style></style>
