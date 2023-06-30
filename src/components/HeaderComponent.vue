<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <!-- <a class="navbar-brand" href="#">DT HOTEL</a> -->
      <a class="navbar-brand" href="#">
            <PixiLogoHeaderComponent />
        </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#"><router-link to="/">Home</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/about">About</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/service">Service</router-link></a>
          </li>
        </ul>
        <div class="d-flex">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/login">Login</router-link></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"><router-link to="/register">Register</router-link></a>
          </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
  </template>

<style>
.wider-navbar {
  width: 100%;
  padding-left: 20px;
  padding-right: 20px;
}
</style>

<script>
import PixiLogoHeaderComponent from '@/components/PixiLogoHeaderComponent.vue'
export default {
  components: {
    PixiLogoHeaderComponent
  }
}
</script>
