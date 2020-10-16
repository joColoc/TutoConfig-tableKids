<template>
  <q-item 
  v-if="to.length"
  :to="to" 
  >
    <q-item-section avatar>
      <q-icon :name="icon" />
    </q-item-section>
    <q-item-section>
      <q-item-label>{{ title }}</q-item-label>
    </q-item-section>
  </q-item>
        <q-expansion-item 
        v-else 
        :label="title"
        icon="check"  >
            <q-list 
            v-for="tiroir in multi" 
            v-bind:key="tiroir.title" 
            class="q-pl-lg" >
              <q-item :to="tiroir.to" class="q-pl-lg">
                <q-item-section avatar>
                  <q-icon :name="tiroir.icon" />
                </q-item-section>
                <q-item-section>
                  <q-item-label>{{ tiroir.title }}</q-item-label>
                </q-item-section>
              </q-item>
            
            </q-list>
          </q-expansion-item>
</template>

<script>
export default {
  name: "MontagePlaqueComponents",
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
    },
    multi: {
      type: Array,
    },
  }
};
</script>
