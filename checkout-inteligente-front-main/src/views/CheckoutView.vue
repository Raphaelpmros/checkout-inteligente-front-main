<script setup>
import CheckoutCard from '../components/checkout/CheckoutCard.vue';
</script>

<template>
  <div class="container">
    <div class="container text-center">
      <h1>Checkout</h1>
      <div class="row">
        <div class="col p-0">
          <div class="mb-3">
            <CheckoutCard nome="Enviar para o meu endereço - Sedex" valor="R$22,90" />
          </div>
          <div class="mb-3">
            <CheckoutCard nome="Enviar para o meu endereço - Entrega convêncional" valor="R$14,80" />
          </div>
          <div class="mb-3">
            <CheckoutCard nome="Retirar na agência mais próxima" valor="R$7,60" />
          </div>
        </div>
        <div class="col-4 p-0 m-5">
          <div class="card col-md-7">
            <div class="card-body">
              <h5 class="card-title">Resumo da compra:</h5>
            </div>
            <label for="forma_pagamento">Escolha a forma de pagamento:</label>
            <select id="forma_pagamento" name="forma_pagamento">
              <option value="cartao_credito">Cartão de Crédito</option>
              <option value="boleto_bancario">Boleto Bancário</option>
              <option value="transferencia_bancaria">Transferência Bancária</option>
              <option value="dinheiro">Dinheiro</option>
            </select>
            <ul class="list-group list-group-flush">
              <li class="list-group-item">Maleta - R$:600,00</li>
              <li class="list-group-item">
                Vara de pesca - R$1450,00
              </li>
              <li class="list-group-item">Total: 2050,00</li>
            </ul>
            <div class="card-body">
              <button type="button" class="btn btn-success">
                <div class="row">
                  <RouterLink to="checkout" class="btn btn-sucess" style="color: white">Finalizar compra</RouterLink>
                </div>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
  
