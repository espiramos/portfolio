<template>
  <div class="flex justify-center items-center text-center">
    <div
      class="
        font-general-regular
        text-lg text-ternary-dark
        dark:text-ternary-light
      "
    >
      &copy; {{ copyrightDate }}. Developed with ❤️ by
      <a
        href="https://www.linkedin.com/in/feranmi-olawale-057474165"
        target="__blank"
        class="
          font-general-medium
          text-secondary-dark
          dark:text-secondary-light
          uppercase
          hover:underline hover:text-indigo-600
          dark:hover:text-indigo-300
          duration-500
        "
        >{{ author }}</a
      >
    </div>
  </div>
</template>

<script>
import { mapState } from "vuex";

export default {
  data: () => {
    return {
      author: "Feranmi",
    };
  },
  computed: {
    ...mapState(["copyrightDate"]),
  },
};
</script>

<style lang="scss" scoped></style>
