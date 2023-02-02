<template>
  <q-layout view="lHh Lpr fFf">
    <q-page-container>
      <q-page>
        <div class="column items-center q-pt-lg">
          <h4 class="text-weight-medium">👋 Hello, World!</h4>

          <p class="text-subtitle1 text-grey-7">Bora aprender sobre web3! Conecta sua wallet e manda um salve pra nós!</p>

          <q-btn push :loading="loading" color="secondary" @click="wave" icon="waving_hand" label="Mandar salve"></q-btn>
        </div>
      </q-page>
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from 'vue'

export default {
  name: 'LayoutDefault',
  data() {
    return {
      loading: ref(false)
    }
  },
  methods: {
    wave() {
      this.loading = true;
    }
  }
}
</script>
