<template>
  <div id="app">
    <HelloWorld :msg="msg">
      new button nam
    </HelloWorld>
    <BaseContent>
    <div class="header-section">
      <template #header>
       header slot template here
      </template>
    </div>
    <div class="section-about-template">
        <template v-slot:sectionAbout>
         section about template here
        </template>
    </div>
    <div class="slot-three">
        <template v-slot:>
          slot three here
        </template>
    </div>
    </BaseContent>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import BaseContent from './components/BaseComponent.vue'
// by the way slot can contains names so you can identify the place where you wanna display you data
/*
the challenge right here is to apply this idea in order to refactor two different context by using slots 

we have a treeview and we need make the needed changes to reach this goal of having one unique Treeview and different way of implementation by calling slots places 

*/
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data(){
    return {
      msg: 'something new'
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
