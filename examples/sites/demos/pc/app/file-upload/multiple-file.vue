<template>
  <tiny-file-upload :action="action" :multiple="true">
    <template #trigger>
      <tiny-button type="primary">选取文件</tiny-button>
    </template>
  </tiny-file-upload>
</template>

<script lang="jsx">
import { FileUpload, Button } from '@opentiny/vue'

export default {
  components: {
    TinyFileUpload: FileUpload,
    TinyButton: Button
  },
  data() {
    return {
      action: 'http://localhost:3000/api/upload'
    }
  }
}
</script>
