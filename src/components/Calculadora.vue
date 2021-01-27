<template>
  <div class="calculadora">
      <div class="display">{{ current }}</div>
      <div class="btn">C</div>
      <div class="btn">+/-</div>
      <div class="btn">%</div>
      <div class="btn operadores">/</div>
      <div class="btn">7</div>
      <div class="btn">8</div>
      <div class="btn">9</div>
      <div class="btn operadores">x</div>
      <div class="btn">4</div>
      <div class="btn">5</div>
      <div class="btn">6</div>
      <div class="btn operadores">-</div>
      <div class="btn">1</div>
      <div class="btn">2</div>
      <div class="btn">3</div>
      <div class="btn operadores">+</div>
      <div class="btn zero">0</div>
      <div class="btn">.</div>
      <div class="btn operadores">=</div>
  </div>
</template>

<script>
export default {
    name: 'Calculadora',
    data() {
        return {
            current: '0',
        }
    }
}
</script>
<style scoped>
.calculadora {
    margin: 0 auto;
    width: 400px;
    font-family: sans-serif;
    font-size: 40px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: minmax(50px auto);
}

.display {
    grid-column: 1/5;
    background-color: #333;
    color: #fff;
}
.zero {
    grid-column: 1/3;
}
.btn {
    background-color: #eee;
    border: 1px solid #999;
}
.operadores {
    background-color: orange;
    color: #fff;
}
</style>