<template>
<div class="grid grid-cols-2 md:grid-cols-3 gap-4">
    <div
      v-for="skill in skills"
      class="flex justify-center items-center"
    >
      <div class="flex flex-col items-center">
        <component
          :is="skill.icon" 
          :width="50"
          :height="50"
        />
        <p class="text-lg font-semibold text-sky-200 mb-8">
          {{ skill.name }}
        </p>
      </div>
    </div>
</div>

</template>

<script>
import {reactive} from 'vue'
import HtmlIcon from './icons/HtmlIcon.vue'
import CssIcon from './icons/CssIcon.vue'
import BootstrapIcon from './icons/BootstrapIcon.vue'
import TailwindIcon from './icons/TailwindIcon.vue'
import JavaScriptIcon from './icons/JavaScriptIcon.vue'
import AstroIcon from './icons/AstroIcon.vue'
import VueIcon from './icons/VueIcon.vue'
import ReactIcon from './icons/ReactIcon.vue'
import WordpressIcon from './icons/WordpressIcon.vue'
import FigmaIcon from './icons/FigmaIcon.vue'
import AngularIcon from './icons/AngularIcon.vue'
import PhpIcon from './icons/PhpIcon.vue'
import LaravelIcon from './icons/LaravelIcon.vue'
import MySqlIcon from './icons/MySqlIcon.vue'
import GitIcon from './icons/GitIcon.vue'
export default {
  components: {
    HtmlIcon,
    CssIcon,
    BootstrapIcon,
    TailwindIcon,
    JavaScriptIcon,
    AstroIcon,
    VueIcon,
    ReactIcon,
    WordpressIcon,
    FigmaIcon,
    AngularIcon,
    PhpIcon,
    LaravelIcon,
    MySqlIcon,
    GitIcon,
  },
  setup () {
    const skills = reactive({
      'HTML':{
        'name': 'HTML',
        'icon': HtmlIcon,
      },
      'CSS':{
        'name': 'CSS',
        'icon': CssIcon,
      },
      'Bootstrap':{
        'name': 'Bootstrap',
        'icon': BootstrapIcon,
      },
      'Tailwind':{
        'name': 'Tailwind CSS',
        'icon': TailwindIcon,
      },
      'JavaScript':{
        'name': 'JavaScript',
        'icon': JavaScriptIcon,
      },
      'Astro':{
        'name': 'Astro',
        'icon': AstroIcon,
      },
      'Vue':{
        'name': 'Vue',
        'icon': VueIcon,
      },
      'React':{
        'name': 'React',
        'icon': ReactIcon,
      },
      'Wordpress':{
        'name': 'Wordpress',
        'icon': WordpressIcon,
      },
      'Figma':{
        'name': 'Figma',
        'icon': FigmaIcon,
      },
      'Angular':{
        'name': 'Angular',
        'icon': AngularIcon,
      },
      'Php':{
        'name': 'PHP',
        'icon': PhpIcon,
      },
      'Laravel':{
        'name': 'Laravel',
        'icon': LaravelIcon,
      },
      'MySql':{
        'name': 'MySql',
        'icon': MySqlIcon,
      },
      'Git':{
        'name': 'Git',
        'icon': GitIcon,
      },
    })
    return {
      skills,
    }
  }
}
</script>

<style scoped>

</style>