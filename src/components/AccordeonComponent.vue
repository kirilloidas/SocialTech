<template>
  <div class="accordion" id="accordionExample">
    <div class="accordion-item" v-for="(item, index) of data" :key="index">
      <h2 class="accordion-header" id="headingOne">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" :data-bs-target="'#collapse' + index" aria-expanded="true" :aria-controls="'collapse' + index">
          {{ item.title }}
        </button>
      </h2>
      <div :id="'collapse' + index" class="accordion-collapse collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
        <ul class="secondary-list">
          <li class="secondary-list__item" v-for="(secondaryItem, secondaryIndex) of item.secondaryList" :key="secondaryIndex">
            {{ secondaryItem }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script setup>
import {reactive} from 'vue'
const data = reactive([
  {
    title: 'The analysis',
    secondaryList: [
      'Do you have one user in more than one variant of the same AB test?',
      'Are you users actually getting the treatment we expect them to get?',
      'Do we have enough users in our AB test? Are those users representative for the total population?'
    ]
  },
  {
    title: 'Our data',
    secondaryList: [
      'Do you have one user in more than one variant of the same AB test?',
      'Are you users actually getting the treatment we expect them to get?',
      'Do we have enough users in our AB test? Are those users representative for the total population?'
    ]
  },
  {
    title: 'Our study case',
    secondaryList: [
      'Do you have one user in more than one variant of the same AB test?',
      'Are you users actually getting the treatment we expect them to get?',
      'Do we have enough users in our AB test? Are those users representative for the total population?'
    ]
  },
  {
    title: 'Hands on analyzing',
    secondaryList: [
      'Do you have one user in more than one variant of the same AB test?',
      'Are you users actually getting the treatment we expect them to get?',
      'Do we have enough users in our AB test? Are those users representative for the total population?'
    ]
  },
  {
    title: 'Initialization',
    secondaryList: [
      'Do you have one user in more than one variant of the same AB test?',
      'Are you users actually getting the treatment we expect them to get?',
      'Do we have enough users in our AB test? Are those users representative for the total population?'
    ]
  }
])
</script>
<style lang="css" scoped>
.accordion {
  width: 600px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.02), 0px 4px 17px rgba(0, 0, 0, 0.14), 0px 4px 22px rgba(0, 0, 0, 0.12);
  border-radius: 8px;
  margin-left: auto;
  margin-right: auto;
}
.accordion-button {
  color: #2B41B7;
  background: #FAF8F6;
  font-style: normal;
  font-weight: 800;
  font-size: 16px;
  line-height: 24px;
  box-shadow: 0 0 0 0 rgba(0, 0, 0, 0) !important;
  padding: 24px 31px 0 24px;
}
.accordion-button.collapsed {
  background: white;
  color: #0D2A54;
  padding: 24px 31px 24px 24px;
}
.collapse, .collapsing {
  background: #FAF8F6;
  padding: 8px 24px 24px 12px;
}
.secondary-list {
  list-style-image: url('../assets/bullet.svg');
  margin-bottom: 0;
}
.secondary-list__item {
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 24px;
}
.secondary-list__item:not(:last-child) {
  margin-bottom: 8px;
}

@media screen and (max-width: 600px) {
  .accordion {
    width: 500px;
  }
}
@media screen and (max-width: 500px) {
  .accordion {
    width: 400px;
  }
}
@media screen and (max-width: 400px) {
  .accordion {
    width: 300px;
  }
}
</style>