<template>
  <v-app>
    <NavBar :links="links" />
    <v-content>
      <router-view />
    </v-content>
    <Footer :links="links" />
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld'
import NavBar from '@/components/NavBar.vue'
import Footer from '@/components/Footer.vue'
export default {
  name: 'App',

  components: {
    // HelloWorld
    NavBar,
    Footer
  },
  data: () => ({
    links: [
      {
        label: 'Home',
        name: 'Home'
      },
      {
        label: 'Login',
        name: 'Login'
      },
      {
        label: 'Signup',
        name: 'Signup'
      },
      {
        label: 'vote',
        name: 'Vote'
      },
      {
        label: 'voting',
        name: 'Voting'
      },
      {
        label: 'Auth',
        name: 'Auth'
      },
      {
        label: 'Dashboard',
        name: 'Dashboard'
      }
    ]
  })
}
</script>
