<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <PixiLogoHeaderComponent/>
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#"><router-link to="/">Home</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#"><router-link to="/about">About</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#"><router-link to="/service">Service</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled"><router-link to="/login">Login</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled"><router-link to="/login"><router-link to="/register">Register</router-link></router-link></a>
        </li>
      </ul>
    </div>
  </div>
</nav>
</template>
<script>
import PixiLogoHeaderComponent from '@/components/PixiLogoHeaderComponent.vue'
export default{
  components:{
    PixiLogoHeaderComponent
  }
}
</script>