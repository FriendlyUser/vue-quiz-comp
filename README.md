# vue_quiz_comp

Basic Quiz Component, to run you can do something simple such as shown in `App.vue`

```vue
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
```

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
