<template>
    <div class="loader-container">
      <div class="loader"></div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'LoaderComponent'
  }
  </script>
  
  <style>
  .loader-container {
    width: 100%;
    height: 100vh;
    background-color: gray;
    opacity: 0.7;
    position: absolute;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 99;
  }
  
  .loader {
    border: 16px solid #f3f3f3;
    border-top: 16px solid #3498db;
    border-radius: 50%;
    width: 120px;
    height: 120px;
    animation: spin 2s linear infinite;
    bottom: 45%;
    position: absolute;
    left: 45%;
  }
  
  @keyframes spin {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }
  </style>
  