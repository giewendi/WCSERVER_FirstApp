<template>
  <div id="app">
    <h1><br><br>{{ name }} | <img id="pic" src="./assets/pic.jpg" alt="Profile Picture"> | {{major}} <br><br><br>{{title}}</h1>
    
    <profile></profile>
    <education></education>
    <skill></skill>

  </div>
</template>

<script>
import Profile from './components/Profile'
import Education from './components/Education'
import Skill from './components/Skill'

export default {
  name: 'app',
  components: {
    Profile,
    Education,
    Skill
  },
  data () {
    return {
      name: 'Giewen D. Pinlac',
      major: 'Web Developer',
      title: 'Resume / CV',
    }
  }
}
</script>

<style>
body{
  margin: 0;
  background-color: rgb(238, 216, 190);
  font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

h1 {
    background: #9adbb3 url('./assets/head.jpg');
    padding: 1em;
    text-align: center;
    margin: 0em 0 -1em 0;
}

#pic{
    height: 125px;
    border-radius: 100%;
    filter: drop-shadow(0 0 1.2px rgb(155, 155, 155));
    margin: 1em 0 -.7em 0;
}

h2{
    background-color: rgb(255, 255, 255);
    padding: 8px;
    filter: drop-shadow(0 0 1px rgb(61, 49, 34));
    text-align: center;
}


</style>