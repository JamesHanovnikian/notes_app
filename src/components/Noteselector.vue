<template>
  <div class="note-selector" v-bind:class="{active: mynote.id === selectedNoteId}"
    v-on:click="selectNote(mynote)">
     <p class="note-selector-title"> {{ mynote.body }}</p>
     <p class="note-selector-timestamp"> {{ mynote.timestamp}} </p>
     <h2> {{selectedNoteId}} </h2>
  </div>
</template>


<script>
export default {
  props: ["mynote", "selectedNoteId"],
  methods: {
    selectNote: function (mynote) {
      console.log(mynote.id);
      this.$emit("selectNote", mynote);
    },
  },
};
</script> 