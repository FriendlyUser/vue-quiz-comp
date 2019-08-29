<template>
  <div id="app">
    <Quiz v-bind:quizObj="{questions: [ { 
      text: 'Who is the Batman',
      responses: [
           {
              text: 'Laughing Bat'
           },
           {
              text: 'Bruce Wayne',
              correct: true
           },
           {
              text: 'Dick Grayson'
           },
           {
              text: 'None of the above'
           }
        ]
    }, {
      text: 'this quiz is fun',
      responses: [
        {
          text: 'Bruce Wayne',
          correct: true
        },
      ]
    } ]}"/>
  </div>
</template>

<script>
import Quiz from './components/Quiz.vue'
export default {
  name: 'app',
  components: {
    Quiz
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
