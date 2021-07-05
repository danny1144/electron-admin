<template>
  <div class="flex flex-row text-center bg-gray-300 ">
    <router-link class="block w-1/2 bg-pink-300 border  border-separate " to="/">首页</router-link>
    <router-link class="block w-1/2 bg-pink-300 border  border-separate" to="/about"> 关于</router-link>
  </div>
  <router-view />
</template>


<script lang="ts">
import Nav from './components/Nav.vue'
import NavItem from './components/Navitem.vue'
import List from './components/List.vue'
import ListItem from './components/ListItem.vue'
export default {
  props: ['recipes'],
  components: {
    Nav,
    NavItem,
    List,
    ListItem,
  },
}

</script>
 
