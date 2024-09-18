<template>
  <v-btn class="ma-2" color="secondary" @click="expand2 = !expand2">
    Expand X Transition
  </v-btn>

  <v-expand-x-transition>
    <v-card
      v-show="expand2"
      class="mx-auto bg-secondary box"
      height="100"
      width="100"
    ></v-card>
  </v-expand-x-transition>
  <v-expand-x-transition>
    <v-card
      v-show="expand2"
      class="mx-auto bg-secondary box"
      height="100"
      width="100"
    ></v-card>
  </v-expand-x-transition>
  <v-expand-x-transition>
    <v-card
      v-show="expand2"
      class="mx-auto bg-secondary box"
      height="100"
      width="100"
    ></v-card>
  </v-expand-x-transition>
</template>
<script>

  export default {
    data: () => ({
      expand2: false,
      elementInView: true,
    }),

    mounted() {
      const observer = new IntersectionObserver(entries => {
        entries.forEach(entry => {
          console.log(entry)
          if (entry.isIntersecting) {
            this.expand2 = true
          } else {
            this.expand2 = false
          }
        })
      })

      const hiddenElements = document.querySelectorAll('.box')
      hiddenElements.forEach(el => observer.observe(el))
    },
  }
</script>
<style>
  .box {
    margin-bottom: 900px;
  }
</style>
