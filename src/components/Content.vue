<template>
  <div id="app">
    <button type="button" class="btn" @click="showModal">
      Open Modal!
    </button>

    <Modal v-show="isModalVisible" @close="closeModal" />
  </div>
</template>

<script>
import Modal from "./Modal.vue";

export default {
  name: "Content",
  components: {
    Modal
  },
  data() {
    return {
      isModalVisible: false
    };
  },
  methods: {
    showModal() {
      this.isModalVisible = true;
    },
    closeModal() {
      this.isModalVisible = false;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.btn {
  padding: 10px;
  font-family: open-sans;
  font-weight: bold;
  font-size: 14;
  margin: 0 auto;
  color: white;
  background: #4aae9b;
  border: 1px solid #4aae9b;
  border-radius: 2px;
  margin-bottom: 20px;
}
</style>
