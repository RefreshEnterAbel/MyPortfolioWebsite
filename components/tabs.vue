<template>
  <div class="qualification__container container">
    <div class="qualification__tabs">
      <template v-for="{tabName,tabIcon,active} in tabs">
        <div class="qualification__button button--flex " :class="{'qualification__active': active}"
             @click="toggleTab(tabName)">
          <i class="uil qualification__icon" :class="tabIcon"/>
          {{ tabName }}
        </div>
      </template>
    </div>
    <div class="qualification__sections">
      <template v-for="{tabContent} in tabs.filter((tab) => tab.active)">
        <div class="qualification__content tabContent">
          <div class="qualification__data" v-for="(data,index) in tabContent">
            <template v-if="(index%2) === 0">
              <div>
                <h3 class="qualification__title" v-text="data.title"/>
                <span class="qualification__subtitle" v-html="data.subtitle"/>
                <div class="qualification__calendar">
                  <i class="uil uil-calendar-alt"/>
                  {{ data.calendar }}
                </div>
              </div>

              <div>
                <span class="qualification__rounder"></span>
                <span class="qualification__line"></span>
              </div>
            </template>
            <template v-else>
              <div></div>
              <div>
                <span class="qualification__rounder"></span>
                <span class="qualification__line"></span>
              </div>
              <div>
                <h3 class="qualification__title" v-text="data.title"/>
                <span class="qualification__subtitle" v-html="data.subtitle"/>
                <div class="qualification__calendar">
                  <i class="uil uil-calendar-alt"/>
                  {{ data.calendar }}
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
import {ref} from 'vue'

const tabs = ref([
  {
    tabName: 'Education',
    tabIcon: 'uil-graduation-cap',
    active: true,
    tabContent: [
      {
        title: 'BSc. in Computer Science',
        subtitle: 'Chittagong University of Engineering & Technology',
        calendar: 'March, 2015 - September, 2019'
      },
      {
        title: 'Higher Secondary School Certificate',
        subtitle: 'Bir Shreshtha Noor Mohammad Public College',
        calendar: 'July, 2012 - September, 2014'
      },
      {
        title: 'Secondary School Certificate',
        subtitle: 'Bir Shreshtha Munshi Abdur Rouf Public College',
        calendar: ' January, 2010 - May, 2012'
      }
    ]
  },
  {
    tabName: 'Work',
    tabIcon: 'uil-briefcase-alt',
    active: false,
    tabContent: [
      {
        title: 'Web Development',
        subtitle: ' <a href="https://ssd-tech.io/" target="_blank">SSD-Tech Limited</a>',
        calendar: 'September, 2019 - July, 2021'
      },
      {
        title: 'PHP & Laravel Instructor',
        subtitle: 'Bir Shreshtha Noor Mohammad Public College',
        calendar: 'October, 2020 - running'
      },
      {
        title: 'Software Development',
        subtitle: ' <a href="https://www.reddotdigital.net/" target="_blank">Red.Digital IT</a><small>(A subsidiary of Robi Axiata Limited)</small>',
        calendar: ' August, 2021 - Running'
      }
    ]
  }
])

function toggleTab(tabName) {
  tabs.value.forEach((tab) => {
    tab.active = tab.tabName === tabName;
  })
}
</script>

<style scoped>

</style>
