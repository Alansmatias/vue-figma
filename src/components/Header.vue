<template>
    <div class="header">
      <div class="header-group">
        <div class="header-overlap-group">
          <!-- Substituição do GenericAvatarWrapper por SVG -->
          <svg class="generic-avatar" viewBox="0 0 24 24" fill="#EADDFF">
            <path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/>
          </svg>
          
          <!-- Substituição do Icon por SVG (ícone de menu hambúrguer) -->
          <svg class="icon-instance" viewBox="0 0 24 24" fill="#EADDFF">
            <path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z"/>
          </svg>
          
          <div class="text-wrapper">Olá, Alan</div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Header'
  };
  </script>
  
  <style>
  .header {
    height: 390px;
    width: 428px;
  }
  
  .header .header-group {
    height: 390px;
    left: 0;
    top: 0;
    width: 430px;
  }
  
  .header .header-overlap-group {
    background: linear-gradient(90deg, rgba(152, 109, 214, 0.71) 0%, rgba(152, 109, 214, 1) 52%);
    border-radius: 0px 0px 100px 100px;
    height: 390px;
    position: relative;
    width: 428px;
  }
  
  .header .generic-avatar {
    height: 42px;
    width: 42px;
    left: 357px;
    position: absolute;
    top: 32px;
  }
  
  .header .icon-instance {
    height: 38px;
    width: 41px;
    left: 30px;
    position: absolute;
    top: 36px;
  }
  
  .header .text-wrapper {
    color: #ffffff;
    font-family: "Inter-Medium", Helvetica;
    font-size: 36px;
    font-weight: 500;
    left: 38px;
    letter-spacing: 0;
    line-height: normal;
    position: absolute;
    top: 173px;
  }
  </style>



