<template>
  <div id="app">
    <AppLayout>
      <template v-slot:default>
        <AppButton><img src="/images/home.svg" /> Home</AppButton>
      </template>
      <template v-slot:header> I was made with Vue slots! </template>
      <!-- Slot reihenfolge spielt keine Rolle. -->
      <template v-slot:footer>By Robert Baumgartner</template>
    </AppLayout>
  </div>
</template>

<script>
// @ is an alias to /src
import AppButton from '@/components/AppButton.vue';
import AppLayout from '@/components/AppLayout.vue';

export default {
  name: 'Home',
  components: {
    AppButton,
    AppLayout,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
