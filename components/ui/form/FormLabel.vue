<script lang="ts" setup>
import { Label } from '@/components/ui/label';
import { cn } from '@/lib/utils';
import type { LabelProps } from 'radix-vue';
import type { HTMLAttributes } from 'vue';
// import { useFormField } from './useFormField';

const props = defineProps<LabelProps & { class?: HTMLAttributes['class'] }>();

// const { formItemId } = useFormField();
</script>

<template>
    <Label :class="cn(props.class)">
        <slot />
    </Label>
</template>
