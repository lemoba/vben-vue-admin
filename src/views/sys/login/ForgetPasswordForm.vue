<template>
  <template v-if="getShow">
    <h2 class="mb-3 text-2xl font-bold text-center xl:text-3xl enter-x xl:text-left">
      {{ getFormTitle }}
    </h2>
    <Button size="large" block class="mt-4" @click="handleBackLogin">
      返回
    </Button>
  </template>
</template>
<script lang="ts" setup>
  import { Button } from 'ant-design-vue';
  import { useI18n } from '/@/hooks/web/useI18n';
  import { useLoginState } from './useLogin';

  const { t } = useI18n();
  const { handleBackLogin } = useLoginState();
</script>
