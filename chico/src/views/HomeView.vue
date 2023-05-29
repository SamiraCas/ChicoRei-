<script setup>
import { RouterLink, RouterView } from 'vue-router'
import "jquery/dist/jquery.slim.min.js";
import "popper.js/dist/umd/popper.min.js";
import "bootstrap/dist/js/bootstrap.min.js";
</script>

<template>
 <section>
    <nav>
  <ul>
    <li>
    <a href="#" class="logo">
      <img src="img/[chicorei.com][880]apple-icon-180x180.png" alt="logo chico rei.png">
      <span class="nav-item">Bem vindo!</span>
    </a>
  </li>
  <li><a href="#">
    <i class="fas fa-home"></i>
    <span class="nav-item">Home</span>
  </a></li>

  <li><a href="#">
    <i class="fas fa-user"></i>
    <span class="nav-item">Perfil</span>
  </a></li>

  <li><a href="#">
    <i class="fas fa-wallet"></i>
    <span class="nav-item">Carteira</span>
  </a></li>
  <li><a href="#">
    <i class="fas fa-chart-bar"></i>
    <span class="nav-item">Analytcs</span>
  </a></li>
  <li><a href="#">
    <i class="fas fa-tasks"></i>
    <span class="nav-item">Lista</span>
  </a></li>
  <li><a href="#">
    <i class="fas fa-cog"></i>
    <span class="nav-item">Setting</span>
  </a></li>
  <li><a href="#">
    <i class="fas fa-question-circle"></i>
    <span class="nav-item">Help</span>
  </a></li>
  <li><a href="#" class="logout">
    <i class="fas fa-sign-out-alt"></i>
    <span class="nav-item"></span>
  </a></li>
  </ul>
 </nav>

   

  </section>
</template>