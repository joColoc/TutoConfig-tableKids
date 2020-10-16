<template>
  <q-page class="">
    <div class="row q-col-gutter-sm  q-py-sm">
      <div class=" q-pl-lg col-lg-6 col-md-6 col-sm-12 col-xs-12">
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
                <div class="text-h6">Programmation du mini PC</div>
              </q-item-section>
            </q-item>
          </q-card-section>
          <q-card-section class="">
            <q-list bordered class="bg-white text-black">
              <q-item v-for="todo in todos" :key="todo.id">
                <q-item-section avatar>
                  <q-icon name="check" />
                </q-item-section>
                <q-item-section class="text-body1 text-wrap">
                  <q-item-label>{{ todo.todo }}</q-item-label>
                </q-item-section>
              </q-item>
            </q-list>
          </q-card-section>
        </q-card>
      </div>
      <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
        <q-card>
          <q-card-section class="text-h6 q-pb-none">
            <q-item>
              <q-item-section>
                <q-carousel
                  animated
                  v-model="slide"
                  navigation
                  infinite
                  :autoplay="autoplay"
                  arrows
                  transition-prev="slide-right"
                  transition-next="slide-left"
                  @mouseenter="autoplay = false"
                  @mouseleave="autoplay = true"
                >
                  <q-carousel-slide :name="1" img-src="~assets/tk-bk-1.jpg" />
                  <q-carousel-slide :name="2" img-src="~assets/IMG_5047.jpg" />
                  <q-carousel-slide :name="3" img-src="~assets/IMG_5048.jpg" />
                </q-carousel>
              </q-item-section>
            </q-item>
          </q-card-section>
        </q-card>
      </div>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/miseEnPlace"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/motdepasse"
      />
      <br />
    </div>
  </q-page>
</template>

<script>
export default {
  name: "ConfigBase",
  data() {
    return {
      slide: 1,
      autoplay: true,
      todos: [
        {
          id: 1,
          todo: "Allumer le mini PC"
        },
        {
          id: 2,
          todo: "Activer le wifi et entrer le mot de passe : HACKLABOT"
        },
        {
          id: 3,
          todo: "Ajouter le compte : tablekids45@gmail.com "
        },
        {
          id: 4,
          todo: "Mot de passe : tonton123 "
        },
        {
          id: 5,
          todo: "Réglage la langue mettre en francais "
        },
        {
          id: 6,
          todo:
            "Régler l’heure et mettre sur GMT+2 et décocher le fuseau horaire automatique."
        },
        {
          id: 7,
          todo:
            "Ouvrir le Play store : allez dans mes jeux et application télécharger toutes les applications. "
        },
        {
          id: 8,
          todo:
            " Attendre le temps du téléchargement et Vérifier que toutes les applications sont installées. "
        },
        {
          id: 9,
          todo:
            "Installer Custom Navigation bar pour changer la barre de navigation. "
        },
        {
          id: 10,
          todo: " Aller dans Paramètres > Compte > Google : Désactiver tout.  "
        }
      ]
    };
  }
};
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 400px
</style>