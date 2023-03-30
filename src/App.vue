<template class="bg-slate-100 min-h-full w-full">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <div class="bg-slate-100 relative">
    <DemoPage msg="My first Vue Project" />
    <ListComponent  />
    <TableHeader  />
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->

    <FooterComponent  class="absolute -bottom-40" />
  </div>
  </template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import DemoPage from './components/DemoPage.vue';
import FooterComponent from './components/FooterComponent.vue';
import ListComponent from './components/ListComponent.vue';
import TableHeader from './components/TableHeader.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    DemoPage,
    ListComponent,
    TableHeader,
    FooterComponent
}
}
</script>

