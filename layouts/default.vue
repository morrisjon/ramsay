<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" app>
      <v-list>
        <v-list-item
          v-for="(link, i) in links"
          :key="i"
          :to="link.to"
          router
          exact
        >
          <v-list-item-action>
            <!-- <v-icon>{{ item.icon }}</v-icon> -->
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="link.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar color="bg" flat fixed app>
      <h2>Ramsay Innovations</h2>
      <v-app-bar-nav-icon
        class="hidden-md-and-up"
        @click.stop="drawer = !drawer"
      />
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-btn
        v-for="link in links"
        :key="link.title"
        :to="link.to"
        class="hidden-sm-and-down mr-4"
        color="primary"
        nuxt
        text
        >{{ link.title }}</v-btn
      >
      <v-btn
        color="primary"
        class="hidden-sm-and-down"
        large
        depressed
        rounded
        to="/contact"
        nuxt
        >Contact Us</v-btn
      >
    </v-app-bar>
    <v-content>
      <v-container fluid class="pa-0">
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
  export default {
    data() {
      return {
        drawer: false,
        links: [
          {
            title: 'Home',
            to: '/'
          },
          {
            title: 'About',
            to: '/about'
          },
          {
            title: 'Services',
            to: '/services'
          }
        ]
      }
    }
  }
</script>

<style>
  .v-list-item::before {
    background: rgba(21, 101, 192, 1);
  }

  .v-list-item:hover::before {
    opacity: 1;
    background-color: rgba(21, 101, 192, 0.87);
  }
</style>
