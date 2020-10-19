<template>
    <li>
        <a :href="href">
            <i class="fa fa-angle-double-right"></i>
            <slot/>
        </a>
    </li>
</template>

<script>
export default {
    name: 'TheFooterItem',
    props: {
        href: String
    }
}
</script>

<style lang="scss" scoped>
a {
  color: #ffffff;

  &:hover {
    color: #eeeeee;
  }
}

li {
    padding: 3px 0;
    transition: 0.5s all ease;

    &:hover {
      padding: 3px 0;
      margin-left: 5px;
    }
  }

li a i {
    margin-right: 5px !important;
}

</style>