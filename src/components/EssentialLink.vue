<template>
  <q-item clickable :to="transacoes">
    <q-item-section v-if="icon" avatar>
      <q-icon style="color: #2196F3;" :name="icon" clickable :to="transacoes" />
    </q-item-section>

    <q-item-section>
      <q-item-label style="color: #f5f5f5;">{{ title }}</q-item-label>
      <q-item-label style="color: #f5f5f5;" caption>
        {{ caption }}
      </q-item-label>
    </q-item-section>
  </q-item>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "EssentialLink",
  props: {
    title: {
      type: String,
      required: true,
    },

    caption: {
      type: String,
      default: "",
    },

    link: {
      type: String,
      default: "#",
    },

    icon: {
      type: String,
      default: "",
    },
    transacoes: {
      type: String,
      default: ''
    }
  },
});
</script>
