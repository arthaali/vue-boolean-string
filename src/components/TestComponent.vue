<script lang="ts" setup>

type Props = {
  value1?: string | boolean;
  value2?: boolean | string;
};

const props = defineProps<Props>();
</script>

<template>
  <div class="dummy-component">
    <span>
      string | boolean: {{ JSON.stringify(props.value1) }}
    </span>
    <span>
      boolean | string: {{ JSON.stringify(props.value2) }}

    </span>
  </div>
</template>
<style lang="scss">
.dummy-component {
  display: flex;
  flex-direction: column;
}
</style>
