<template>
    <div class="menu-container">
      <div class="menu-card">
        <!-- Botão Comprar Terreno -->
        <div class="menu-item" @click="handleTerrenoClick">
          <svg class="menu-icon" viewBox="0 0 24 24" fill="#291547">
            <path d="M17 12h-5v5h5v-5zM12 7H7v5h5V7z"/> <!-- Ícone de terreno simplificado -->
          </svg>
          <div class="menu-label">Comprar<br>Terreno</div>
        </div>
  
        <!-- Botão Comprar Imóvel (meio) -->
        <div class="menu-item middle-item" @click="handleImovelClick">
          <svg class="menu-icon" viewBox="0 0 24 24" fill="#291547">
            <path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"/> <!-- Ícone de casa -->
          </svg>
          <div class="menu-label">Comprar<br>Imóvel</div>
        </div>
  
        <!-- Botão Quitar -->
        <div class="menu-item" @click="handleQuitarClick">
          <svg class="menu-icon" viewBox="0 0 24 24" fill="#291547">
            <path d="M12 2L4 7v10l8 5 8-5V7L12 2zm0 15.5l-5-3v-5l5 3v5zm1-5v5l5-3v-5l-5 3z"/> <!-- Ícone de pagamento -->
          </svg>
          <div class="menu-label">Quitar</div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Menu1",
    methods: {
      handleTerrenoClick() {
        console.log("Comprar Terreno clicado");
        // this.$emit('terreno-click');
      },
      handleImovelClick() {
        console.log("Comprar Imóvel clicado");
        // this.$emit('imovel-click');
      },
      handleQuitarClick() {
        console.log("Quitar clicado");
        // this.$emit('quitar-click');
      }
    }
  };
  </script>
  
  <style>
  .menu-container {
    width: 334px;
    height: 137px;
    display: flex;
    justify-content: center;
    position: relative;
    top: -20px;
  }
  
  .menu-card {
    background: #FFFFFF;
    border-radius: 23px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 0 10px;
  }
  
  .menu-item {
    background-color: #f5eff7;
    border-radius: 10px;
    width: 97px;
    height: 94px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .menu-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
  }
  
  .menu-icon {
    width: 39px;
    height: 39px;
    margin-bottom: 8px;
  }
  
  .menu-label {
    color: #291547;
    font-family: "Inter-Medium", Helvetica;
    font-size: 12px;
    font-weight: 500;
    text-align: center;
    line-height: 1.3;
  }
  
  .middle-item {
    margin: 0 10px;
  }
  </style>