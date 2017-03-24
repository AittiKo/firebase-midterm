<template lang="html">
  <tbody>
      <tr v-for="(book, index) in books" transition>
        <td>
          {{index + 1}}
        </td>
        <td>
          <a v-bind:href="book.url">{{book.title}}</a>
        </td>
        <td>
          {{book.author}}
        </td>
        <td>
          <span class="glyphicon glyphicon-trash" v-on:click="removebook(book)"></span>
        </td>
      </tr>
      <!-- <nav class="navbar navbar-default">
        <div class="container">
          <div class="navbar-header">
            <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#collapse">
              <span class="sr-only">Toggle navigation</span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              </button>
              <a class="navbar-brand" href="#">WebsiteName</a>
              </div>
              <div class="collapse navbar-collapse" id="collapse">
                <ul class="nav navbar-nav">
                  <li class="active"><a href="#">Page 1</a></li>
                  <li><a href="#">Page 2</a></li>
                  <li><a href="#">Page 3</a></li>
                </ul>
              </div>
            </div>
          </nav> -->
  </tbody>

</template>

<script>
export default {
  props: ['books', 'removebook']
}
</script>

<style lang="css">


</style>
