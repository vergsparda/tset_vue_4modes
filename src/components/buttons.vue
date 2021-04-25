<template>
  <div class="btn">
    <button class="btn-red">1</button>
    <button class="btn-green">2</button>
    <button class="btn-blue">3</button>
    <button class="btn-yellow">4</button>
  </div>
</template>

<script>
export default {
  name: 'app',

}
  // const btnRed = document.querySelector('.btn-red');
  // // const btnGreen = document.querySelector('.btn-green');
  // // const btnBlue = document.querySelector('.btn-blue');
  // // const btnYellow = document.querySelector('.btn-yellow');
  // const html = document.querySelector("html");

  // html.addEventListener('click', (e) => {
  //   if (e === btnRed) {
  //   e.preventDefault();
  //   html.classList.toogle("btn-red");
  //   }
  // })

</script>

<style scoped>
  button {
  box-sizing: border-box;
  width: 100px;
  height: 30px;
}

.btn-red {
  background-color: red;
}

.btn-green {
  background-color: green;
}
.btn-blue {
  background-color: blue;
}

.btn-yellow {
  background-color: yellow;
}
</style>

