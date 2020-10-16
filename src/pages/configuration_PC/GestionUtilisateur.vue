<template>
  <q-page>
    <h4 class="q-pa-lg text-center">Gestion Utilisateur</h4>
    <div class="flex-center row items-start q-gutter-md">
      <q-card class="my-card">
        <q-img src="~assets/user-1.jpg" basic> </q-img>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/user-2.jpg" basic> </q-img>
      </q-card>
      <q-card class="my-card">
        <q-img src="~assets/tk.jpg" basic> </q-img>
      </q-card>

      <q-card-section style="font-size: 17px;">
        Sélectionner le nom d'utilisateur et le modifier par Tous les jeux<br />Puis
        créer un nouvel utilisateur et le nommer
        <strong>Multijoueurs</strong> et
        <strong>Petit -6ans</strong> Sélectionner ces applications.
        <br />
        Puis retourner sur tous les jeux et lancer le test de chaque jeu.
        <br />
        <br />

        Pour ces jeux quitter le contrôle parental car il demande d’accepter
        certaine condition :
        <ul>
          <li>Crossy Road (accepter les photos)</li>
          <li>Cut the rope (accepter les photos)</li>
          <li>Drive Ahead (connexion compte Google Play)</li>
          <li>Skiddy car</li>
          <li>Tic tac toc</li>
          <li>Basketball battle</li>
          <li>Pipe out (accepter les photos)</li>
          <li>
            Maze & more (ouvrir la première fois avec internet activé)
          </li>
        </ul>

        <div>Restauration des achats avec internet :</div>
        <ul>
          <li>Forme et couleur</li>
          <li>Coloriage</li>
          <li>Puzzle de couleur</li>
        </ul>
      </q-card-section>
    </div>

    <!-- button -->
    <div class="q-pa-lg q-gutter-lg flex flex-center">
      <q-btn
        color="secondary"
        icon="keyboard_arrow_left"
        label="Etape precedente"
        to="/parametreInterface"
      />
      <q-btn
        color="red"
        icon-right="keyboard_arrow_right"
        label="Etape suivante "
        to="/extinction"
      />
      <br />
    </div>
  </q-page>
</template>
<script>
export default {
  name: "GestionUtilisateur"
};
</script>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 750px
</style>