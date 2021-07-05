<template>
    <div class="bg-white dark:bg-gray-800">
        <h1 class="text-gray-900 dark:text-white">Dark mode is here!</h1>
        <p class="text-gray-600 dark:text-gray-300">Lorem ipsum...</p>
    </div>
</template>

<script   lang="ts">
import { ref, defineComponent } from 'vue'
export default defineComponent({
    name: 'About',
    props: {
        msg: {
            type: String,
            required: true
        }
    },
    setup: () => {
        const count = ref(0)
        return { count }
    }
})

</script>

<style scoped>
</style>