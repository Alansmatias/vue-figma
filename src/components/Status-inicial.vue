<template>
    <div class="status-inicial">
      <div class="card-container">
        <div class="card-content">
          <div class="property-title">TERRENO LOTEAMENTO VIVA</div>
          <div class="installments">Parcelas restantes: 35/40</div>
          
          <!-- Barra de progresso -->
          <div class="progress-bar">
            <div class="progress-fill"></div>
          </div>
          
          <div class="payment-info">
            <div class="paid-amount">Pagas: R$3.420</div>
            <div class="remaining-amount">Restante: R$86.580</div>
          </div>
          
          <!-- Botões -->
          <div class="buttons-container">
            <button class="details-btn">Detalhes</button>
            <button class="pay-btn">Pagar</button>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'StatusInicial'
  };
  </script>
  
  <style>
  .status-inicial {
    width: 334px;
    height: 198px;
    font-family: "Inter-Medium", Helvetica;
    position: relative;
    top: -50px;
  }
  
  .card-container {
    position: relative;
    width: 100%;
    height: 100%;
    background-color: #ffffff;
    border-radius: 23px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    padding: 20px;
    box-sizing: border-box;
  }
  
  .property-title {
    color: #291547;
    font-size: 20px;
    font-weight: 500;
    margin-bottom: 15px;
  }
  
  .installments {
    color: #291547;
    font-size: 12px;
    margin-bottom: 8px;
  }
  
  .progress-bar {
    background-color: #d9d9d9;
    height: 12px;
    width: 100%;
    border-radius: 6px;
    margin-bottom: 15px;
    overflow: hidden;
  }
  
  .progress-fill {
    background-color: #986dd6;
    height: 100%;
    width: 12%; /* Ajuste conforme o progresso (35/40) */
    border-radius: 6px;
  }
  
  .payment-info {
    display: flex;
    justify-content: space-between;
    margin-bottom: 15px;
    font-size: 12px;
  }
  
  .paid-amount {
    color: #291547;
  }
  
  .remaining-amount {
    color: #291547;
    text-align: right;
  }
  
  .buttons-container {
    display: flex;
    justify-content: space-between;
  }
  
  .details-btn {
    background-color: #f5eff7;
    color: #65558f;
    border: none;
    padding: 8px 16px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 14px;
  }
  
  .pay-btn {
    background-color: #986dd6;
    color: white;
    border: none;
    padding: 8px 24px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 14px;
  }
  </style>