<template>
  <div id="app">
    <link href="https://fonts.googleapis.com/css?family=Lato:300,300i,400,400i,700,700i&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Overpass:300,300i,400,400i,600,600i,700,700i&display=swap" rel="stylesheet">
    <Nav></Nav>
    <h1 class="col-5 mt-4">Mes projets</h1>
    <div class="container-fluid mt-5">
      <div class="row">
        <div class="col-xg-2 col-lg-2"></div>
        <Project></Project>
        <Project></Project>
        <Project></Project>
        <Project></Project>
      </div>
      <div class="row">
        <div class="col-xl-2 col-lg-2"></div>
        <Project></Project>
        <Project></Project>
        <Project></Project>
        <Project></Project>
      </div>
    </div>
  </div>
</template>

<script>
  import Nav from './components/Nav.vue'
  import Project from './components/Project.vue'

export default {
  name: 'app',
  components: {
    Nav,
    Project
  }
}
</script>

<style lang="scss">
  #app{
    font-family: 'Lato', sans-serif;
    font-family: 'Overpass', sans-serif;
    h1{
      color: white;
      border-bottom: #FFF 3px solid;
    }
  }
  body{
    background-color: #323232 !important;
  }
</style>
