<template>
  <tiny-file-upload ref="upload" :data="requestData" :before-upload="beforeUpload">
    <template #trigger>
      <tiny-button type="primary">选取文件</tiny-button>
    </template>
  </tiny-file-upload>
</template>

<script lang="jsx">
import { FileUpload, Button, Modal } from '@opentiny/vue'

export default {
  components: {
    TinyFileUpload: FileUpload,
    TinyButton: Button
  },
  data() {
    return {
      requestData: {
        id: 123
      }
    }
  },
  methods: {
    beforeUpload() {
      Modal.message('查看请求头示例请打开浏览器开发者工具 network 的 upload 请求')
      return true
    }
  }
}
</script>
