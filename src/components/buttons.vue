<template>
  <div class="btn">
    <button v-for="(color, index) in colors" :class="color" :key="index"
            @click="printBack(color)">
    </button>
  </div>
</template>

<script>
export default {
  props: {
    colors: {
      type: Array,
      require: false,
    }
  },

  data() {
    return {
      defaultColors: [],
    };
  },

  computed: {
    trueColors() {
      return this.defaultColors;
    }
  },
  methods: {
    printBack(color){
      const html = document.querySelector("html");
      setTimeout(() => {
        if (html.style.backgroundColor === color) {
          html.style.backgroundColor = "#fff";
        } else {
          html.style.backgroundColor = color
        }
      setTimeout(() => {

      }, )
      }, 1000);

    }
  },
  mounted() {
    setTimeout(() => {
        this.defaultColors = ['red', 'green', 'blue']
    }, 1000)
  }
}


</script>

<style scoped>
  button {
  box-sizing: border-box;
  width: 100px;
  height: 30px;
}

.red {
  background-color: red;
}

.green {
  background-color: green;
}
.blue {
  background-color: blue;
}

.yellow {
  background-color: yellow;
}
</style>

