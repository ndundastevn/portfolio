<template>
    <v-layout>
      <!-- app bar -->
		<v-app-bar
			color="black"
		>
			<template v-if="$vuetify.display.smAndDown">
			<v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
			</template>

			<v-toolbar-title>
			<h2 class="2px ml-12">StevNdunda</h2>
			</v-toolbar-title>

			<v-spacer></v-spacer>

			<template v-if="$vuetify.display.mdAndUp">
			<v-btn @click="scroll('home')" variant="text">Home</v-btn>
			<v-btn @click="scroll('about')" variant="text">About</v-btn>
			<v-btn @click="scroll('skills')" variant="text">skills</v-btn>
			<v-btn @click="scroll('education')" variant="text">education</v-btn>
			<v-btn @click="scroll('education')" variant="text">experience</v-btn>
			<v-btn @click="scroll('portfolio')" variant="text">portfolio</v-btn>
			<v-btn @click="scroll('contact')" variant="text">Contact</v-btn>
			</template>
		</v-app-bar>

      <!-- naviation drower -->
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
        <div class="bg-black">
          <v-container id="home">
            <barner/>
          </v-container>
        </div>

        <!-- About -->
        <v-container id="about">
          <about />
        </v-container>

        <div class="bg-black">
          <!-- Skills -->
          <v-container color="black" id="skills" class="py-16">
              <skills/>
          </v-container>

          <!-- education/experience -->
          <v-container color="black" id="education">
              <education/>
          </v-container>
        </div>

        <!-- portfolio -->
        <v-container id="portfolio">
          <portfolio/>
        </v-container>

        <!-- contact -->
        <v-container id="contact">
          <div>
            <h1 class="text-h2 text-center font-weight-bold mt-12">
              Contact Me
            </h1>
            <v-card class="mt-4" title="Phone" text="08888548545" prepend-icon="mdi-phone" variant="tonal"></v-card>
            <v-card class="mt-4" title="Phone" text="08888548545" prepend-icon="mdi-phone" variant="tonal"></v-card>
          </div>
        </v-container>

      </v-main>
    </v-layout>



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

    methods:{
      scroll(page){
        var elements = document.getElementById(page);
        elements.scrollIntoView();
      }
    },

    watch: {
      group () {
        this.drawer = false
      },
    },

    // mounted() {
    //   // Get the elements with the class name 'contactmepage'
    //   var elements = document.getElementsByClassName('contactmepage');

    //   // Check if there is at least one element with that class
    //   if (elements.length > 0) {
    //     // Scroll the first element into view
    //     elements[0].scrollIntoView();

    //     // Log the element to the console
    //     console.log('element is...', elements[0]);
    //   } else {
    //     console.log('No elements with class contactmepage found.');
    //   }
    // }
  }
</script>

<style>
  a {
    padding-right: 40px;
    font-size: 30px;
    color: white;
    text-decoration: none;
  }
  a:hover {
    color: rgb(40, 167, 69);
  }
  v-btn:hover {
    color: rgb(40, 167, 69);
  }
  h1 {
    color: rgb(40, 167, 69);
    font-family: 'Jost', cursive;
    font-size: 60px;
    font-weight: 600;
  }
  h2 {
    color: rgb(40, 167, 69);
    font-family: 'Jost', cursive;
    /* font-size: 40px; */
    font-weight: 900;
  }
  h4 {
    color: rgb(40, 167, 69);
    font-family: 'Jost', cursive;
    /* font-size: 40px; */
    font-weight: 900;
  }
  h3 {
    font-weight: 700;
    color: rgb(255, 255, 255);
    font-family: 'Jost', cursive;
    font-size: 26px;
    line-height: 36px;
  }
  p {
    color: rgb(255, 255, 255);
    font-family: 'Jost', sans-serif;
    font-size: 20px;
    font-weight: 400;
    line-height: 24px;
  }
  .mytext {
    font-family: 'Jost', sans-serif;
    font-size: 15px;
    font-weight: 400;
    line-height: 24px;
  }
  .parag {
    color: rgb(255, 255, 255);
    font-family: 'Jost', sans-serif;
    font-size: 20px;
    font-weight: 400;
    line-height: 24px;
  }
  .title{
    color: rgb(255, 255, 255);
    font-family: 'Jost', sans-serif;
  }
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    color: aliceblue;
    text-decoration: none;
  }
</style>
