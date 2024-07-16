<template>
  <!-- nav bar -->
  <v-app-bar density="prominent" border-0 class="bg-black">
    <template v-slot:prepend>
      <h2 class="pl-12">StevNdunda</h2>
    </template>

    <template v-slot:append>
      <v-list class="d-flex bg-black" color="black">
        <v-list-item>
          <v-list-title>HOME</v-list-title>
        </v-list-item>
        <v-list-item>
          <v-list-title>ABOUT</v-list-title>
        </v-list-item>
        <v-list-item >
          <v-list-title>CONTACT</v-list-title>
        </v-list-item>
      </v-list>
      <!-- <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#contact" class="pr-40">Contact</a> -->

      <v-btn icon="mdi-dots-vertical"></v-btn>
    </template>

</v-app-bar>
  <!-- end .nav -->

<!-- home -->
<div id="home">
 <v-card
 class="mt-0"
 border-0
 color="black"
 >
  <v-row>
  <v-col cols="6">
  <v-card-title class="mt-12">Hi, there. I'm"</v-card-title>
  <h1 class="pl-4">Stephen Ndunda</h1>
    <v-card-subtitle>Software Engineer, Creative Web Developer, and Graphic Designer </v-card-subtitle>
    <v-card-text>With a passion for crafting innovative solutions and captivating designs, I bring a unique blend of technical expertise and creative flair to every project. Let's bring your ideas to life! </v-card-text>
	<v-card-actions>
  <v-layout column>
    <v-flex>
      <v-icon icon="$vuetify"></v-icon>
      <span>0888858585</span>
    </v-flex>
    <v-flex>
      <v-icon icon="$vuetify"></v-icon>
      <span>0888858585</span>
    </v-flex>
  </v-layout>
</v-card-actions>

  </v-col>
  <v-col cols="6">
    <v-img
        class="mb-4 mt-12"
        height="150"
        src="@/assets/logo.png"
      />
  </v-col>
  </v-row>
</v-card>
</div>
<!-- end card -->

  <v-container class="fill-height">
    <v-responsive
      class="align-centerfill-height mx-auto"
      max-width="1200"
    >
<!-- About me -->
      <div class="text-center" id="about">
        <h1 class="text-h2 font-weight-bold">
          About Me
        </h1>
        <div class="text-body-2 font-weight-light mb-n1 pt-4">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam, quasi soluta natus tempora minus, odit ab adipisci dignissimos sunt cumque eius cupiditate quae hic. Quidem temporibus repellat ex laborum a necessitatibus soluta, exercitationem fugit, molestias adipisci voluptatibus commodi non impedit vitae qui provident eveniet, officia quaerat! Nostrum eos vel suscipit dignissimos libero nesciunt eveniet repellendus odio consequuntur omnis, tenetur, eius nisi perferendis. Laudantium incidunt ipsum asperiores aliquam facilis aspernatur deleniti alias facere rerum dolore debitis eligendi dolorum ullam esse unde animi culpa repellat qui, autem provident sunt eius vero? Dolores porro accusamus ab eaque placeat itaque reiciendis quas debitis labore eos amet eligendi pariatur, ex, vel laudantium, earum facere voluptatibus tenetur iure harum! Recusandae consectetur saepe quos earum totam ipsam, repellat quo qui dolores assumenda accusantium neque iure aperiam similique nulla delectus nobis corrupti libero eos voluptatibus vitae! Saepe facilis, quo magni laborum, excepturi nulla minima, delectus tempora officia natus sunt pariatur et libero laboriosam nihil quibusdam optio aperiam. Doloremque voluptates vero voluptatum natus assumenda, sapiente, dolores iure dolorum ratione consequuntur est, odit fugit. At, maxime ipsam placeat debitis iure, quia, laudantium cum eum assumenda possimus accusantium voluptatum nulla cupiditate non delectus. Ipsum tenetur quod ex culpa nesciunt. Sit totam quae maxime fuga repellat numquam illum exercitationem, autem odit omnis. Ullam in qui aliquam repellat ut voluptatem possimus rem minima temporibus dignissimos, cupiditate, perspiciatis, ratione nisi voluptate. Vel autem commodi perferendis natus nam placeat laudantium iusto. Quisquam labore, sit quae neque hic impedit perferendis? Ipsa quaerat itaque adipisci inventore facilis veniam, aperiam quia saepe quae error eius autem voluptatem, voluptatum voluptate minima sapiente ex vero eligendi placeat? Odit, ab suscipit eaque dolorum placeat et ea qui ipsum quas maiores deserunt aliquam atque minima, iure corrupti esse dolores, nisi consequatur officia. Officiis in maiores sint nihil ipsa praesentium pariatur error consectetur.
        </div>

      </div>

      <!-- What i do -->
      <div class="text-center my-12">
        <h1 class="text-h2 font-weight-bold">
          What I do
        </h1>


		<v-card
		class="py-4 mt-6"
		color="surface-variant"
		rounded="lg"
		variant="outlined"
		>

            <template #title>
              <h2 class="text-h5 font-weight-bold">Software, Web and Mobile Development</h2>
            </template>

            <template #text>
              <div class="text-subtitle-1">
				As a software developer, I specialize in creating efficient and reliable applications that have responsive features. My focus is on ensuring that the apps I build can adapt to any screen size. I make sure to consider the overall project goals while understanding my clients' needs, and am able to quickly create prototypes. I also use efficient development methods and tools to give my clients a competitive edge.
              </div>
            </template>

            <v-overlay
              opacity=".12"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
		<v-card
		class="py-4 mt-6"
		color="surface-variant"
		rounded="lg"
		variant="outlined"
		>

            <template #title>
              <h2 class="text-h5 font-weight-bold">Software, Web and Mobile Development</h2>
            </template>

            <template #text>
              <div class="text-subtitle-1">
				        As a software developer, I specialize in creating efficient and reliable applications that have responsive features. My focus is on ensuring that the apps I build can adapt to any screen size. I make sure to consider the overall project goals while understanding my clients' needs, and am able to quickly create prototypes. I also use efficient development methods and tools to give my clients a competitive edge.
              </div>
            </template>

            <v-overlay

              opacity=".12"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>


      </div>

      <!-- technical / professional skills -->
      <v-row>
        <v-col cols="6">
          <h1 class="text-h2 font-weight-bold">
            Technical / Professional Skills
          </h1>
          <p>PHP - Laravel / codeIgniter</p>
          <v-progress-linear color="primary" class="mb-4" model-value="20"></v-progress-linear>
          <p>PHP - Laravel / codeIgniter</p>
          <v-progress-linear color="primary" class="mb-4" model-value="20"></v-progress-linear>
          <p>PHP - Laravel / codeIgniter</p>
          <v-progress-linear color="primary" class="mb-4" model-value="20"></v-progress-linear>
          <p>PHP - Laravel / codeIgniter</p>
          <v-progress-linear color="primary" class="mb-4" model-value="20"></v-progress-linear>
        </v-col>
        <v-col cols="6">
          <h1 class="text-h2 font-weight-bold">
            Soft Skills
          </h1>
          <div class="flex">
            <v-progress-circular
              color="primary"
              model-value="20"
              :size="83"
              :width="11"
            >90%</v-progress-circular>

            <v-progress-circular
              color="primary"
              model-value="20"
              :size="83"
              :width="11"
            ></v-progress-circular>
            <br/>
            <v-progress-circular
  color="primary"
  model-value="20"
  :size="83"
  :width="11"
></v-progress-circular>
<v-progress-circular
  color="primary"
  model-value="20"
  :size="83"
  :width="11"
></v-progress-circular>
          </div>
        </v-col>
      </v-row>

      <!-- Work experience and education -->
      <v-row>
        <v-col cols="8">
          <h1 class="text-h2 font-weight-bold">
            Work Experience
          </h1>
          <v-card title="Card title" class="mt-6" variant="tonal">
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nam corporis cumque eligendi? Quod accusantium corrupti dolorem repudiandae? Odit eligendi necessitatibus ut dicta deleniti, dignissimos perferendis vero eius voluptates amet ab officia cupiditate iste sit magni distinctio quas, sint mollitia rerum optio culpa pariatur tempore. A architecto inventore, autem numquam sunt dolorem neque unde aspernatur quae suscipit perspiciatis accusantium sapiente doloribus voluptatibus nihil nulla error illum officia ullam. Dolorem cupiditate a ipsum provident commodi sequi, quae asperiores rem magni ea cum laboriosam! Obcaecati deleniti incidunt dicta sapiente pariatur saepe alias impedit non. Enim accusamus odit aliquid exercitationem officia iste labore sunt?
            </v-card-text>
          </v-card>
          <v-card title="Card title" class="mt-6" variant="tonal">
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nam corporis cumque eligendi? Quod accusantium corrupti dolorem repudiandae? Odit eligendi necessitatibus ut dicta deleniti, dignissimos perferendis vero eius voluptates amet ab officia cupiditate iste sit magni distinctio quas, sint mollitia rerum optio culpa pariatur tempore. A architecto inventore, autem numquam sunt dolorem neque unde aspernatur quae suscipit perspiciatis accusantium sapiente doloribus voluptatibus nihil nulla error illum officia ullam. Dolorem cupiditate a ipsum provident commodi sequi, quae asperiores rem magni ea cum laboriosam! Obcaecati deleniti incidunt dicta sapiente pariatur saepe alias impedit non. Enim accusamus odit aliquid exercitationem officia iste labore sunt?
            </v-card-text>
          </v-card>
          <v-card
            append-icon="mdi-open-in-new"
            class="py-4 mt-6"
            color="surface-variant"

            prepend-icon="mdi-text-box-outline"
            rel="noopener noreferrer"
            rounded="lg"
            text="Learn about all things Vuetify in our documentation."
            target="_blank"
            title="Documentation"
            variant="text"
          >
            <v-overlay
              opacity=".06"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
        </v-col>


        <v-col cols="4">
          <h1 class="text-h2 font-weight-bold">
            Education
          </h1>
          <v-card title="Card title" class="mt-6" variant="tonal">
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit.
            </v-card-text>
          </v-card>
          <v-card title="Card title" class="mt-6" variant="tonal">
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit.
            </v-card-text>
          </v-card>
          <v-card title="Card title" class="mt-6" variant="tonal">
            <v-card-text>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit.
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>

      <!-- projects -->
  <v-card class="mt-12">
    <v-tabs
      v-model="tab"
      align-tabs="center"
      color="deep-purple-accent-4"
    >
      <v-tab :value="1">Landscape</v-tab>
      <v-tab :value="2">City</v-tab>
      <v-tab :value="3">Abstract</v-tab>
    </v-tabs>

    <v-tabs-window v-model="tab">
      <v-tabs-window-item
        v-for="n in 3"
        :key="n"
        :value="n"
      >
        <v-container fluid>
          <v-row>
            <v-col
              v-for="i in 6"
              :key="i"
              cols="12"
              md="4"
            >
              <v-img
                :lazy-src="`https://picsum.photos/10/6?image=${i * n * 5 + 10}`"
                :src="`https://picsum.photos/500/300?image=${i * n * 5 + 10}`"
                height="205"
                cover
              ></v-img>
            </v-col>
          </v-row>
        </v-container>
      </v-tabs-window-item>
    </v-tabs-window>
  </v-card>
<!-- .end projects -->

<!-- contact me -->
<div class="text-center my-12" id="contact">
    <h1 class="text-h2 font-weight-bold">
      Contact Me
    </h1>
    <v-card

      class="mx-auto"

      prepend-icon="mdi-github"

      subtitle="088558585"

      title="Phone"
    ></v-card>
</div>
<!-- ./end contact me -->
      <v-img
        class="mb-4"
        height="150"
        src="@/assets/logo.png"
      />


      <div class="text-center">
        <div class="text-body-2 font-weight-light mb-n1">Welcome to</div>

        <h1 class="text-h2 font-weight-bold">Vuetify</h1>
      </div>

      <div class="py-4" />

      <v-row>
        <v-col cols="12">
          <v-card
            class="py-4"
            color="surface-variant"
            image="https://cdn.vuetifyjs.com/docs/images/one/create/feature.png"
            prepend-icon="mdi-rocket-launch-outline"
            rounded="lg"
            variant="outlined"
          >
            <template #image>
              <v-img position="top right" />
            </template>

            <template #title>
              <h2 class="text-h5 font-weight-bold">Get started</h2>
            </template>

            <template #subtitle>
              <div class="text-subtitle-1">
                Replace this page by removing <v-kbd>{{ `<HelloWorld />` }}</v-kbd> in <v-kbd>pages/index.vue</v-kbd>.
              </div>
            </template>

            <v-overlay
              opacity=".12"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
        </v-col>

        <v-col cols="6">
          <v-card
            append-icon="mdi-open-in-new"
            class="py-4"
            color="surface-variant"
            href="https://vuetifyjs.com/"
            prepend-icon="mdi-text-box-outline"
            rel="noopener noreferrer"
            rounded="lg"
            subtitle="Learn about all things Vuetify in our documentation."
            target="_blank"
            title="Documentation"
            variant="text"
          >
            <v-overlay
              opacity=".06"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
        </v-col>

        <v-col cols="6">
          <v-card
            append-icon="mdi-open-in-new"
            class="py-4"
            color="surface-variant"
            href="https://vuetifyjs.com/introduction/why-vuetify/#feature-guides"
            prepend-icon="mdi-star-circle-outline"
            rel="noopener noreferrer"
            rounded="lg"
            subtitle="Explore available framework Features."
            target="_blank"
            title="Features"
            variant="text"
          >
            <v-overlay
              opacity=".06"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
        </v-col>

        <v-col cols="6">
          <v-card
            append-icon="mdi-open-in-new"
            class="py-4"
            color="surface-variant"
            href="https://vuetifyjs.com/components/all"
            prepend-icon="mdi-widgets-outline"
            rel="noopener noreferrer"
            rounded="lg"
            subtitle="Discover components in the API Explorer."
            target="_blank"
            title="Components"
            variant="text"
          >
            <v-overlay
              opacity=".06"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
        </v-col>

        <v-col cols="6">
          <v-card
            append-icon="mdi-open-in-new"
            class="py-4"
            color="surface-variant"
            href="https://discord.vuetifyjs.com"
            prepend-icon="mdi-account-group-outline"
            rel="noopener noreferrer"
            rounded="lg"
            subtitle="Connect with Vuetify developers."
            target="_blank"
            title="Community"
            variant="text"
          >
            <v-overlay
              opacity=".06"
              scrim="primary"
              contained
              model-value
              persistent
            />
          </v-card>
        </v-col>
      </v-row>
    </v-responsive>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      tab: null,
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
  font-size: 40px;
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
