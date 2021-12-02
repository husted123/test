<template>
  <div class="modal-background" @click="close">
    <div class="modal" @click.stop="">
      <header class="modal-header">
        <h5 style="margin: 0 auto">This is my modal</h5>
        <button type="button" class="btn-close" @click="close">X</button>
      </header>
      <section class="modal-body">
        <p>
          Click on confirm, X or outside this modal to close it!
        </p>
      </section>
      <footer class="modal-footer">
        <button type="button" class="btn-cta" @click="close">
          Confirm
        </button>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  name: "Modal",
  methods: {
    close() {
      this.$emit("close");
    }
  }
};
</script>

<style>
.modal-background {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.3);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1;
}

.modal {
  background: #ffffff;
  box-shadow: 2px 2px 20px 1px;
  overflow-x: auto;
  display: flex;
  flex-direction: column;
  z-index: 2;
}

.modal-header,
.modal-footer {
  padding: 10px;
  display: flex;
}

.modal-header {
  position: relative;
  border-bottom: 1px solid #eeeeee;
  background-color: #212121;
  color: #f2f2f2;
}

.modal-footer {
  flex-direction: column;
  justify-content: flex-end;
  background-color: #212121;
  color: #f2f2f2;
}

.modal-body {
  position: relative;
  padding: 20px 20px;
}

.btn-close {
  position: absolute;
  top: 0;
  right: 0;
  border: none;
  font-size: 20px;
  padding: 10px;
  cursor: pointer;
  font-weight: bold;
  color: #00b2a9;
  background: transparent;
}

.btn-cta {
  font-family: open-sans;
  font-weight: bold;
  font-size: 14;
  margin: 0 auto;
  color: white;
  background: #4aae9b;
  border: 1px solid #4aae9b;
  border-radius: 2px;
  width: 20%;
}
</style>
