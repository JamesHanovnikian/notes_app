<template>
  <div class="note-container">
    <Noteselectors />
      <div class="note-editor">
        <p class="note-editor-info">Timestamp here...</p>
        <textarea class="note-editor-input">
          First note...

          Note text here...
        </textarea>
      </div>
    </div>
</template>

<script>
import Noteselectors from "./Noteselectors.vue";
export default {
  components: {
    Noteselectors,
  },
};
</script> 