<template>
  <div class="container">
    <div class="row mt-4">
      <div class="col text-center">
        <h1 class="light">Markdown Preview</h1>
      </div>
    </div>

    <div class="row mut-4">
      <div class="col-md-5">
        <h4 class="light">Markdown</h4>
        <textarea
          class="info"
          v-model="markdown"
        />
      </div>
      <div class="col-md-5">
        <h4 class="light">Preview</h4>
        <div 
          class="info">
          {{markdown}}
        </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      markdown: '',
    }
  }
}
</script>

<style scoped>
textarea {
  resize: none;
  border: 1px dashed orange;
  outline: none;
}
.info {
  height: 400px;
  width: 100%;
  background-color: rgba(255, 255, 255, 0.9);
}
</style>
