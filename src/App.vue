<template>
  <div id="app">
    <div class="row">
      <div class="col-md-4 col-md-offset-4">
        <img src="./assets/cat.jpg" class="img-circle center-block">
        <h1>{{ msg }}</h1>
        <h1>{{msg1}}</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Moooooday',
      msg1:"Every Day is Moday"
    }
  }
}
</script>
