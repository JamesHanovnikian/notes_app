<template>
  <div class="note-selector active">
     <p class="note-selector-title"> {{ mynote.body }}</p>
     <p class="note-selector-timestamp"> {{ mynote.timestamp}} </p>
  </div>
</template>


<script>
export default {
  props: ["mynote"],
};
</script> 