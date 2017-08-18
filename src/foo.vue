<template>
  <div class="wrapper" @click="update">
    <image :src="logoUrl" class="logo"></image>
    <text class="title">Hello {{target}}</text>
    <div class="">
      <a class="button" href="https://angel.co/jobs">
        <text class="text">Angel.co</text>
      </a>
    </div>
  </div>
  
</template>

<style>
  .wrapper { align-items: center; margin-top: 120px; }
  .title { font-size: 48px; }
  .logo { width: 360px; height: 82px; }
</style>

<script>
  export default {
    data: {
      logoUrl: 'https://alibaba.github.io/weex/img/weex_logo_blue@3x.png',
      target: 'My name is Madhu Nandi'
    },
    methods: {
      update: function (e) {
        this.target = 'Weex'
        console.log('target:', this.target)
      }
    }
  }
</script>
