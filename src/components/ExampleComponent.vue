<script>
export default {
  data() {
    return {
      isRed: true
    };
  },

  /*
   * Same as
   * <template>
   *   <div :class="{'is-red': isRed}">
   *     <p>Example Text</p>
   *   </div>
   * </template>
   */
  render(h) {
    return h(
      "div",
      {
        class: {
          "is-red": this.isRed
        }
      },
      [h("p", "Example Text")]
    );
  }
};
</script>