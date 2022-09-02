<template>
  <div class="skills__container container grid">
    <div>
      <template v-for="skill in skills">
        <div class="skills__content" :class="{'skills__open': skill.open,'skills__close': !skill.open}">
          <div class="skills__header" @click="toggleSkills(skill.title)">
            <i class="uil uil-brackets-curly skills__icon"/>
            <div>
              <h1 class="skills__title" v-text="skill.title"/>
              <span class="skills__subtitle" v-text="skill.experience"/>
            </div>

            <i class="uil uil-angle-down skills__arrow"/>
          </div>
          <div class="skills__list grid">
            <template v-for="tool in skill.tools">
              <div class="skills__data">
                <div class="skills__titles">
                  <h3 class="skills__name" v-text="tool.name"/>
                  <div class="skills__number" v-text="`${tool.level}%`"/>
                </div>
                <div class="skills__bar">
                  <div class="skills__percentage" :style="`width: ${tool.level}%`"/>
                </div>
              </div>
            </template>
          </div>
        </div>
      </template>
    </div>
  </div>
</template>

<script setup>
import {ref} from "vue";

const skills = ref([
  {
    title: 'Backend Development',
    experience: 'More than 2 years',
    open: true,
    tools: [
      {
        name: 'Laravel',
        level: 80
      },
      {
        name: 'PHP',
        level: 80
      },
      {
        name: 'Django',
        level: 60
      },
      {
        name: 'Typescript',
        level: 70
      },
    ]
  },
  {
    title: 'Frontend Development',
    experience: 'More than 1 years',
    open: false,
    tools: [
      {
        name: 'React.js',
        level: 80
      },
      {
        name: 'Material UI',
        level: 80
      },
      {
        name: 'Javascript',
        level: 60
      },
      {
        name: 'Formik',
        level: 70
      },
    ]
  },
  {
    title: 'Database Design',
    experience: 'More than 2 years',
    open: false,
    tools: [
      {
        name: 'MySQL',
        level: 80
      },
      {
        name: 'Graphql',
        level: 80
      },
      {
        name: 'Javascript',
        level: 60
      },
      {
        name: 'Formik',
        level: 70
      },
    ]
  }
])

function toggleSkills(skillName) {
  skills.value.forEach((skill) => {
    if (skill.title === skillName) skill.open = !skill.open
  })
}
</script>

<style scoped>

</style>
