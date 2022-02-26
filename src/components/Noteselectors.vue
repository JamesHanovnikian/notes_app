<template>
  <div class="note-selectors">
    <Noteselector 
    v-for="note in notes" 
    v-bind:key="note.id"
    v-bind:mynote="note"
    /> 
  </div>
</template>



<script>
import Noteselector from "./Noteselector.vue";

export default {
  components: {
    Noteselector,
  },
  data: function () {
    return {
      notes: [
        { id: 1, body: "Note 1", timestamp: Date.now() },
        { id: 2, body: "Note 2", timestamp: Date.now() },
        { id: 3, body: "Note 3", timestamp: Date.now() },
      ],
    };
  },
};
</script> 