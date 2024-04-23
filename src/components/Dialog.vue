<script>
export default {
  name: "cagh-dialog",
  methods: {
    open() {
      this.$refs.dialog.show();
    },
  },
};
</script>

<template>
  <dialog ref="dialog">
    <div class="grid gap">
      <slot></slot>
      <form method="dialog">
        <button>Ok</button>
      </form>
    </div>
  </dialog>
</template>