<template>
  <div class="home">
    <div class="canvas-container" ref="canvasDom"></div>
  </div>
</template>

<script setup>
import * as THREE from "three";
// import { onMounted,reactive, ref } from "vue";

//创建场景
const scene = new THREE.Scene()
//创建相机
const camera = new THREE.PerspectiveCamera(
  75,window.innerWidth/window.innerHeight,
  0.1,
  1000
);
camera.position.set(0,2,6)

//创建渲染器
const renderer = new THREE.WebGLRenderer()


</script>

<style>

</style>
