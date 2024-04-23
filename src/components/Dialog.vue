<script>
export default {
  name: "cagh-dialog",
  methods: {
    open() {
      this.$refs.dialog.showModal();
    },
  },
};
</script>

<template>
  <dialog ref="dialog">
    <div class="grid gap">
      <slot></slot>
      <form method="dialog">
        <button filled>Ok</button>
      </form>
    </div>
  </dialog>
</template>