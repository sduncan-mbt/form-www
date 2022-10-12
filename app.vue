<template>
  <div>
    <form @click.prevent="formSubmitted=true">
      <input type="text" />
    </form>
    <h1>{{formSubmitted}}</h1>
  </div>
</template>
<script setup>
import {useState} from "nuxt/app";

const formSubmitted = useState('formSubmitted', () => false)
</script>
