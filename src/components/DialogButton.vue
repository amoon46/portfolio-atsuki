<template>
  <div class="text-center">
    <v-hover v-slot:default="{ isHovering, props }" open-delay="100">
      <v-card
        :elevation="isHovering ? 16 : 2"
        @click="dialog = true"
        v-bind="props"
        class="pa-2"
      >
        <v-img
          :src="kaedeImage"
        ></v-img>
      </v-card>
    </v-hover>

    <v-dialog v-model="dialog" width="auto">
      <DialogCard :showDialog="dialog" @update:showDialog="dialog = $event" />
    </v-dialog>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import DialogCard from './../components/DialogCard'
import kaedeImage from './../assets/kaede.jpg'

const dialog = ref(false)
</script>
