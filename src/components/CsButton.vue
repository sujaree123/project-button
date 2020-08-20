<template>
  <div>
    <button v-on:click="upFunction" class="genric-btn primary circle ml-3 mt-10">
      <span class="text-black fas fa-thumbs-up"> Like</span>
    </button>

    <button v-on:click="downFunction" class="genric-btn success circle ml-3 mt-10">
      <span class="text-black fas fa-laugh-beam"> Takecare</span>
    </button>

    <button v-on:click="loveFunction" class="genric-btn info circle ml-3 mt-10">
      <span class="text-black fas fa-heart"> Love</span>
    </button>

    <button v-on:click="dislikeFunction" class="genric-btn circle warning ml-3 mt-10">
      <span class="text-black fas fa-thumbs-down"> Dislike</span>
    </button>

    <button v-on:click="ResetFunction" class="genric-btn danger circle ml-3 mt-10">
      <span class="text-black fas fa-redo-alt"> Reset</span>
    </button>
  </div>
</template>

<script>
export default {
  name: "CSButton",
  data: function () {
    return {
      counter: 0,
    };
  },
  methods: {
    upFunction: function () {
      this.counter += 5;
      this.$emit("cc", this.counter);
    },

    downFunction: function () {
      this.counter += 20;
      this.$emit("cc", this.counter);
    },

    loveFunction: function () {
      this.counter += 10;
      this.$emit("cc", this.counter);
    },

    dislikeFunction: function () {
      this.counter -= 15;
      this.$emit("cc", this.counter);
    },

    ResetFunction: function () {
      this.counter = 0;
      this.$emit("cc", this.counter);
    },
  },
};
</script>

<style>
</style>