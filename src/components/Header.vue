<template>
    <header>
      <h1>{{ title }}</h1>
      <Button text="Add Task" color="green"/>
    </header>
  </template>

<script>
import Button from './Button'

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: 'Header',
    props: {
        title: String,
        },
        components: {
            Button
        }
    }

</script>

<style scoped>
 header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333;
    color: #fff;
    padding: 10px;
    border-radius: 5px;
    margin-bottom: 20px;
 }
</style>