<template lang="html">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h3>Add book</h3>
    </div>
    <div class="panel-body">
      <form id="form" class="form-inline" v-on:submit.prevent="addbook">
        <div class="form-group">
          <label for="bookTitle">Title:</label>
          <input type="text" id="bookTitle" class="form-control" v-model="newbook.title">
        </div>
        <div class="form-group">
          <label for="bookAuthor">Author:</label>
          <input type="text" id="bookAuthor" class="form-control" v-model="newbook.author">
        </div>
        <div class="form-group">
          <label for="bookUrl">URL:</label>
          <input type="text" id="bookUrl" class="form-control" v-model="newbook.url">
        </div>
        <input type="submit" class="btn btn-primary" value="Add Book">
      </form>
    </div>
  </div>
</template>

<script>
export default {
  props: ['addbook', 'newbook']
}
</script>

<style lang="css">
</style>
