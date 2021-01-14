<template>
  <div>
      <h1>{{message}}</h1>
      <p>Page no {{number}}</p>
      <button @click=callGoogle()>click me</button>
  </div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        message: {
            type: String,
            default: "Hello my name is header"
        },
        number: {
            type: Number,
            required: true
        }
    },
    methods: {
        callGoogle(){
            // alert("hey you called this method");
            window.location ="https://google.com";
        }
    }
}
</script>

<style>

</style>