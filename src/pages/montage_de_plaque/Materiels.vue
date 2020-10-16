<template>
  <q-page>
    <h4 class=" q-pa-lg text-center">Matériels nécessaires</h4>
    <div class="q-pa-md flex flex-center items-start q-gutter-md">
      <q-card v-for="(item, index) in Materials" :key="item.id" class="my-card">
        <q-img :src="Materials[index].image" basic>
          <div class="absolute-bottom text-subtitle2 text-center">
            {{ Materials[index].item }}
          </div>
        </q-img>
      </q-card>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/cables"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  data() {
    return {
      Materials: [
        {
          id: 1,

          item: "Une plaque",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 2,

          item: "Cable usb type B",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 3,

          item: " Rallonge USB ",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 4,

          item: "Cable RJ45",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 5,

          item: "Un suppoprt pour fixer l'ordinateur",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 6,

          item: "Un suppoprt pour fixer l'ordinateur",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 7,

          item: "Un suppoprt pour fixer l'ordinateur",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 8,

          item: "Un suppoprt pour fixer l'ordinateur",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 9,

          item: "Un suppoprt pour fixer l'ordinateur",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        },
        {
          id: 10,

          item: "Un suppoprt pour fixer l'ordinateur",

          image: "https://cdn.quasar.dev/img/parallax2.jpg"
        }
      ]
    };
  }
};
</script>

<style lang="sass" scoped>
.my-card
  width: 400px
  max-width: 250px
</style>