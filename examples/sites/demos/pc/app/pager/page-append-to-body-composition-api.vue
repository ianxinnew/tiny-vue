<template>
  <tiny-pager
    :popper-append-to-body="false"
    layout="sizes,prev, pager, next"
    :page-size="5"
    :page-sizes="[5, 10, 20, 30, 40, 50, 100]"
    :total="50"
  ></tiny-pager>
</template>

<script setup lang="jsx">
import { Pager as TinyPager } from '@opentiny/vue'
</script>
