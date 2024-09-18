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
			<h2 class="ml-xm-0">StevNdunda</h2>
			</v-toolbar-title>

			<v-spacer></v-spacer>

			<template v-if="$vuetify.display.mdAndUp">
			<v-btn @click="scroll('home')" variant="text">Home</v-btn>
			<v-btn @click="scroll('about')" variant="text">About</v-btn>
			<v-btn @click="scroll('skills')" variant="text">skills</v-btn>
			<v-btn @click="scroll('education')" variant="text">education</v-btn>
			<v-btn @click="scroll('education')" variant="text">experience</v-btn>
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
        <div class="bg-black hidden" >
          <v-container id="home">
            <barner/>
          </v-container>
        </div>

        <!-- About -->
        <v-container id="about" class="hidden">
          <about />
        </v-container>

        <div class="bg-black hidden" >
          <!-- Skills -->
          <v-container color="black" id="skills" class="py-16">
              <skills/>
          </v-container>

          <!-- education/experience -->
          <v-container color="black wow zoomIn" data-wow-delay="0.1s" id="education">
              <education/>
          </v-container>
        </div>

        <!-- contact -->
        <v-container id="contact" class="hidden">
          <contact/>
        </v-container>

      </v-main>
    </v-layout>



</template>

<script>
import contact from '@/components/contact.vue';


  export default {
  components: { contact },
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
