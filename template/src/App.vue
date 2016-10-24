<template>
  <v-app navbar footer>
    <header>
      <v-navbar>
        <div class="navbar__logo">Welcome</div>
        <v-navbar-items>
          <v-navbar-item
            class="navbar__item--active"
            v-bind:item="item"
          >
          </v-navbar-item>
        </v-navbar-items>
      </v-navbar>
    </header>
      <main>
        <h1>Vuetify</h1>
        <h2>Essential Links</h2>
        <div class="intro">
          <v-list>
            <v-list-item>
              <v-list-item-title>
                <a href="http://vuetifyjs.com">Vuetify Documentation</a>
              </v-list-item-title>
            </v-list-item>
          </v-list>
          <v-list>
            <v-list-item>
              <v-list-item-title>
                <a href="http://vuejs.org">VueJS Documentation</a>
              </v-list-item-title>
            </v-list-item>
          </v-list>
        </div>
      </main>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        item: {
          href: '#!',
          text: 'Get Started'
        }
      }
    },

    mounted () {
      this.$vuetify.init()
    }
  }
</script>

<style{{#sass}} lang="scss"{{/sass}}>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>

<style lang="stylus">
  @import './stylus/main'
</style>
