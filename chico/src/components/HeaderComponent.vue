<script setup>

</script>
<template>
     <section>
        <div class="img-banner">
          <img src="img/[chicorei.com][580]97277bf0-f95f-11ed-a13a-45af67468193.png" alt="[chicorei.com][580]97277bf0-f95f-11ed-a13a-45af67468193.png">
        </div>
        <div class="img-desconto">
          <img src="img/[chicorei.com][118]primeira-compra.png" alt="[chicorei.com][118]primeira-compra.png">
        </div>
       </section>
</template>

<style  scoped>
@import './base.css'; 
@import url('https://fonts.googleapis.com/css2?family= Poppins:wght@300;400;500;600família= Poppins:wght@300;400;500;700 & =swap');

*{
  margin: 0 ;
  padding: 0;
  overflow-x: hidden;
  outline: none;
  border: none;
  text-decoration: none;
  box-sizing: border-box;
  font-family:"Poppins", sans-serif;
}
boby{
  background: #dfe9f5;
}
nav{
  position: fixed;
  top: 0;
  bottom: 0;
  height: 200%;
  left: 0;
  background: #FFF;
  width: 90px;
  overflow: hidden;
  transition: width 0.2s linear;
  box-shadow: 0 20px 35px rgba(0, 0, 0, 0.1);
}

.logo{
  text-align: center;
  display: flex;
  transition: all 0.5s ease;
  margin: 10px 0 0 10px;
}

.logo img{
  width: 50px;
  height: 50px;
  border-radius: 50%;
}
.logo span{
  font-weight: bold;
  padding-left: 15px;
  font-size: 18px;
  text-transform: uppercase;
}
a{
  position: relative;
  color: rgb(85, 83, 83);
  font-size: 14px;
  display: table;
  width: 300px;
  padding: 10px;
}
.fas{
  position: relative;
  width: 70px;
  height: 40px;
  font-size: 20px;
  text-align: center;
}
.nav-item{
  position: relative;
  top: 10px;
  margin-left: 10px;
  text-align: center;
}
a:hover{
  background: #eee;
}
nav:hover{
  width: 280px;
  transition: all 0.5 ease;
}
.logout{
  position: fixed;
  bottom: 0;
}

.img-banner img{
  align-items: center;
  margin: 0% 60% 0% 15% ;
  
}

.img-desconto img{
  align-items: center ;
  margin: 0% 60% 0% 15% ;
}






</style>