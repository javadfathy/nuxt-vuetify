<script setup>
const colors =  ref([
          'indigo',
          'warning',
          'pink darken-2',
          'red lighten-1',
          'deep-purple accent-4',
        ])
const slides = ref([
    'First',
    'Second',
    'Third',
    'Fourth',
    'Fifth',
])
</script>

<template>
    <section class="text-center ">
        <h1>nuxt and vuetify starter kits</h1>
        <h3>created by javad fathi</h3>
        <h4><a href="https://github.com/javadfathy">my github</a></h4>
        <VCarousel height="400"
                    show-arrows="hover"
                    cycle
                    hide-delimiter-background>
            <VCarouselItem v-for="(slide, i) in slides"
                            :key="i">
                            <VSheet
                                :color="colors[i]"
                                height="100%"
                            >
                                <div class="d-flex fill-height justify-center align-center">
                                <div class="text-h2">
                                    {{ slide }} Slide
                                </div>
                                </div>
                            </VSheet>
            </VCarouselItem>
        </VCarousel>
    </section>
</template>