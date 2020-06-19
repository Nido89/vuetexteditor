<template>

  <div id="app">
    <h1 >TextEditor for Eximia</h1>
   <TextEditor id="myeditor"/>
  </div>
</template>

<script>
import TextEditor from './components/TextEditor.vue'

export default {
  name: 'App',
  components: {
    TextEditor
  }
}
</script>

<style>
body{
  
  background-color: teal;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color:black;
  margin:0 0 60px;

}
  h1{
    color: white;
}
#myeditor{
  background-color: white;
}
</style>
