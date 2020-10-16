<template >
  <div class="q-col-gutter-sm  q-py-lg">
    <div class="flex flex-center col-lg-6 col-md-6 col-sm-12 col-xs-12">
      <q-card class="bg-blue text-white">
        <q-card-section class="text-h6 q-pb-none">
          <q-item>
            <q-item-section avatar>
              <q-icon
                color="white"
                name="library_add_check"
                style="font-size: 2em;"
              />
            </q-item-section>

            <q-item-section>
              <div class="text-h6">
                Vérification des paramétres de configuration
              </div>
            </q-item-section>
          </q-item>
        </q-card-section>
        <q-card-section class="">
          <q-list bordered class="bg-white text-black">
            <q-item v-for="todo in todos" :key="todo.id">
              <q-item-section avatar>
                <q-checkbox
                  :id="todo.id"
                  v-model="todo.completed"
                  color="primary"
                />
              </q-item-section>
              <q-item-section
                class="text-body1 text-wrap"
                :style="
                  todo.completed ? { textDecoration: 'line-through' } : {}
                "
              >
                <q-item-label>{{ todo.todo }}</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
        </q-card-section>
      </q-card>
    </div>

    <!--button-->
    <div class="q-pa-lg q-ma-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/extinction"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "Verification",
  data() {
    return {
      todos: [
        {
          id: 1,
          completed: false,
          todo: "Vérifier si le WiFi s'éteint au démmarage du contrôle parental"
        },
        {
          id: 2,
          completed: false,
          todo: "Vérifier si les pub et le bouton retour sont désactivés"
        },
        {
          id: 3,
          completed: false,
          todo: " Vérifier si le code est 1357"
        },
        {
          id: 4,
          completed: false,
          todo:
            "Vérifier si les comptes sont : Tous les jeux, Multijoueur et Petit -6ans"
        },
        {
          id: 5,
          completed: false,
          todo:
            "Vérifier si lorsqu'on allume et éteint, le contrôle parental se lance"
        },
        {
          id: 6,
          completed: false,
          todo: "Vérifier si il y a au moins 30 jeux fonctionels"
        },
        {
          id: 7,
          completed: false,
          todo: " Vérifier la barre de navigation"
        },
        {
          id: 7,
          completed: false,
          todo: "Vérifier si dans Comptes > Google : tous est décochés"
        },
        {
          id: 7,
          completed: false,
          todo:
            "Vérifier si le fond d'écran est appliqué sur le bureau et le bureau du contrôle parental"
        },
        {
          id: 7,
          completed: false,
          todo: " Vérifier la date et l'heure"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>
