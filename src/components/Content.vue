<template>
  <div>
    <Button/>
    <Modal/>
    <h1>{{ msg }}</h1>
    
  </div>
</template>

<script>
import Button from './Button'
import Modal from './Modal'
export default {
  props: {
    msg: String
  },
  components: {
    Button,
    Modal
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
