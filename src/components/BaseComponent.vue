<template>
<div class="main-content">
  <div class="header">
    this  is  the header slot
    <slot name="header"></slot>
  </div>
  <div class="section-about">
    this is the section-about slot
    <slot name="sectionAbout"></slot>
  </div>
  <div class="sidebar-upcoming-events">
    this is the section upcoming-events slot
    <slot name="sidebar"></slot>
  </div>
</div>
<template>

<script>
export default{
  props:{

  },
  data(){
    return {
      slopProprs:{

      }
    }
  },
  created(){

  },
  methods:{

  }
}
<script>
<style>
</style>