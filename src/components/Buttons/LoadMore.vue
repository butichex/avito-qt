<template>
    <div class="button load-more">
        {{ text }}
    </div>
  </template>
  
  <script lang="ts">
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    name: 'LoadMore',
    props: {
      text: String,
    },
  });
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped lang="scss">
    .load-more {
        cursor: pointer; 
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: 'Roboto';
        font-size: 0.75rem;
        color: #072D4B;
        padding: 0.5rem 0.8rem;
        border: 0.2px solid #072D4B;
        border-radius: 0.25rem;
        background-color: transparent;
        transition: all 0.1s  ease-in;
    }


    .load-more:hover {
        background-color: #072D4B; 
        color: white;
    }
  </style>
  