<template>
    <li>
        <router-link
            :href="href"
            :class="['block px-4 py-2 rounded-md', { 'bg-amber-100 text-amber-700': isActive }]"
        >
            <slot></slot>
        </router-link>
    </li>
</template>
  
  <script lang="ts">
export default {
    props: {
        href: {
            type: String,
            required: true,
        },
        isActive: Boolean,
    },
}
</script>
  
  