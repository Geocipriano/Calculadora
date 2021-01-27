<template>
  <div class="calculadora">
      <div class="display">Teste</div>
      <div>C</div>
      <div>+/-</div>
      <div>%</div>
      <div>+</div>
      <div>7</div>
      <div>8</div>
      <div>9</div>
      <div>x</div>
      <div>4</div>
      <div>5</div>
      <div>6</div>
      <div>-</div>
      <div>1</div>
      <div>2</div>
      <div>3</div>
      <div>+</div>
      <div class="zero">0</div>
      <div>.</div>
      <div>=</div>
  </div>
</template>

<script>
export default {
    name: 'Calculadora'
}
</script>
<style scoped>
.calculadora {
    font-family: sans-serif;
    font-size: 40px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-auto-rows: minmax(50px auto);
}

.display {
    grid-column: 1/5;
    background-color: aquamarine;
}
.zero {
    grid-column: 1/3;
}
</style>