<template>
  <q-item :to="to">
    <q-item-section avatar>
      <q-icon :name="icon" />
    </q-item-section>
    <q-item-section>
      <q-item-label>{{ title }}</q-item-label>
    </q-item-section>
  </q-item>
</template>

<script>
export default {
  name: "EssentialLink",
  props: {
    title: {
      type: String,
      required: true
    },
    to: {
      type: String,
      required: true
    },

    icon: {
      type: String,
      default: ""
    }
  }
};
</script>
