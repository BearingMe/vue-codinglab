<template>
  <li class="list-inline-item">
    <a :href="href">
      <div
        class="d-flex justify-content-center align-items-center"
        :style="`background: ${color}`"
      >
        <slot />
      </div>
    </a>
  </li>
</template>

<script>
export default {
  name: "TheFooterSocial",

  props: {
    href: String,
    color: String,
  },
};
</script>

<style lang="scss" scoped>
div {
  color: #ffffff;
  border-radius: 50%;
  width: 40px;
  height: 40px;

	i {
		font-size: 18px;
	}
}
</style>