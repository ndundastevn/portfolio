<template>
          <a href="#contact" variant="text">Contact</a>

  <v-card>
    <v-layout>
      <v-app-bar
        color="black"
        border-0
      >
        <template v-if="$vuetify.display.smAndDown">
          <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        </template>

        <v-toolbar-title>
          <h2 class="2px">StevNdunda</h2>
        </v-toolbar-title>

        <v-spacer></v-spacer>

        <template v-if="$vuetify.display.mdAndUp">
          <v-btn href="#about" variant="text">Home</v-btn>
          <v-btn href="#about" variant="text">About</v-btn>
          <v-btn href="#skills" variant="text">skills</v-btn>
          <v-btn href="#contact" variant="text">Contact</v-btn>

          <v-btn icon="mdi-filter" variant="text"></v-btn>
        </template>

      </v-app-bar>

      <v-navigation-drawer
        v-model="drawer"
        :location="$vuetify.display.mobile ? 'left' : undefined"
        temporary
      >
        <v-list
          :items="items"
        ></v-list>
      </v-navigation-drawer>

      <v-main>
        <!-- banner -->


          <barner/>


        <v-container>
          <!-- About -->
          <about />

        </v-container>

        <!-- education/experience -->
        <div class="bg-black">
          <v-container color="black">
              <skills/>
              <education/>
          </v-container>
        </div>

        <!-- portfolio -->
        <v-container>
          <portfolio/>
        </v-container>

        <!-- contact -->
        <div class="contact">
        <contact/>

        </div>

      </v-main>
    </v-layout>
  </v-card>
  <div class="contact">
    <h1>hello world</h1>
  </div>
</template>

<script>
  export default {
    data: () => ({
      drawer: false,
      group: null,
      items: [
        {
          title: 'Foo',
          value: 'foo',
        },
        {
          title: 'Bar',
          value: 'bar',
        },
        {
          title: 'Fizz',
          value: 'fizz',
        },
        {
          title: 'Buzz',
          value: 'buzz',
        },
      ],
    }),

    mounted() {
      this.scrollToHome();
    },
    methods: {
        scrollToHome() {
            const homeElement = this.$el.querySelector('#home');
            if (homeElement) {
                homeElement.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        }
    },

    watch: {
      group () {
        this.drawer = false
      },
    },
  }
</script>

<style>
a{
  padding-right: 40px;
  font-size: 30px;
  color: white;
  text-decoration: none;
}
a:hover{
  color: rgb(40, 167, 69);
}
h1{
  color: rgb(40, 167, 69);
  font-family: "Jost", cursive;
  font-size: 60px;
  font-weight: 600;
}
h2{
  color: rgb(40, 167, 69);
  font-family: "Jost", cursive;
  /* font-size: 40px; */
  font-weight: 900;
}
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  color:aliceblue;
  text-decoration: none;
}
</style>

