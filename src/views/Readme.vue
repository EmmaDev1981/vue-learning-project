<template>
  <div class="about">
    <h1>{{ counter }}</h1>
    <button @keyup.enter="decrement"> - 1 </button>
    <button @click="increment"> + 1 </button>
  </div>
</template>

<script>
export default {

  data() {
    return {
      counter: 5
    }

  },
  methods: {
    increment() {
      this.counter = this.counter + 5
    },
    decrement() {
      this.counter = this.counter - 5
    }
  }
  

}



</script>