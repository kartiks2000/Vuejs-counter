<template>
  <div>
    <h3>child counter: {{count}}</h3>
    <button @click="inc1">Increment</button>
    <button @click="dec1">Decrement</button>
  </div>
</template>

<script>
export default {
  props: ["count"],
  methods:{
      inc1(){
          this.$emit("incit",1);
      },
      dec1(){
          this.$emit("decit",1);
      }
  }
}
</script>

<style scoped>
    div{
        text-align: center;
    }
</style>