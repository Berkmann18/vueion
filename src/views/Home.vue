<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary">
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content padding>
      <ion-list>
        <ion-item>
          <ion-checkbox slot="start"></ion-checkbox>
          <ion-label>
            <h1>Create Idea</h1>
            <ion-note>Run Idea by Brandy</ion-note>
          </ion-label>
          <ion-badge color="success" slot="end">5 Days</ion-badge>
        </ion-item>
      </ion-list>
      <ion-fab vertical="bottom" horizontal="end" slot="fixed">
        <ion-fab-button @click="$router.push({ name: 'new-item' })">
          <ion-icon name="add" />
        </ion-fab-button>
      </ion-fab>
    </ion-content>
  </ion-page>
</template>

<script>
import { add } from 'ionicons/icons';
import { addIcons } from 'ionicons';

addIcons({
  'ios-add': add.ios,
  'md-add': add.md
});

export default {
  name: 'Home',
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
