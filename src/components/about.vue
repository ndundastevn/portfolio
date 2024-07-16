<template>
<!-- About me -->
  <div class="py-16 my-12" id="about">
    <h1 class="text-h2 text-center font-weight-bold">
      About Me
    </h1>

    <p class="pt-12 parag text-medium-emphasis">
      Experienced Software Engineer with a robust background spanning over 6 years, specializing in Linux and Unix cloud architectures and administration. My expertise extends to developing resilient solutions across diverse landscapes, using Java, PHP, Python, Ruby and C++. I have a strong foundation in industry-leading frameworks such as Spring Boot, Flask, Django, Laravel, Code Igniter and ASP.NET.
    </p>
    <p class="pt-6 parag text-medium-emphasis">I excel in project management and agile methodologies, ensuring efficient team collaboration and adapting to evolving project requirements. My experience includes working with Content Management Systems (CMS) like WordPress and Wix, and proficiently managing SQL databases (MySQL, Microsoft SQL Server) and NoSQL databases (MongoDB, PostgreSQL, Redis). </p>
    <p class="pt-6 parag text-medium-emphasis">As a versatile full-stack developer, I prioritize User Interface (UI) and User Experience (UX) best practices, leveraging tools like Adobe XD and Figma for optimal design, also my expertise in version control ensures streamlined collaboration and effective code management throughout the development process. </p>
  </div>

  <!-- What i do -->
  <div class="text-center my-16 py-12">
    <h1 class="text-h2 font-weight-bold">
      What I do
    </h1>

    <!-- card -->
		<v-card
		class="py-4 mt-12"
		color="surface-variant"
		rounded="lg"
		variant="outlined"
		>
      <template #title>
        <h2 class="text-h5 font-weight-bold">Software, Web and Mobile Development</h2>
      </template>

      <template #text>
        <div class="text-subtitle-1 parag text-medium-emphasis">
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
    <!-- card -->
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
        <div class="text-subtitle-1 parag text-medium-emphasis">
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
    <!-- card -->
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
        <div class="text-subtitle-1 parag text-medium-emphasis">
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


</template>

<style>
#about{
  color: rgb(255, 255, 255);
  font-family: "Jost", sans-serif;
  font-size: 20px;
  font-weight: 400;
  line-height: 24px;
  opacity: 0.9;
  text-align: center;
}
</style>
