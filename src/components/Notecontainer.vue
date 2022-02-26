<template>
  <div class="note-container">
    <Noteselectors />
    <Noteeditor /> 
    </div>
</template>

<script>
import Noteselectors from "./Noteselectors.vue";
import Noteeditor from "./Noteeditor.vue";
export default {
  components: {
    Noteselectors,
    Noteeditor,
  },
};
</script> 