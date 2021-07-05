<template>
    <div>
        <button class="bg-red-500 hover:bg-red-700 ...">Hover me</button>
    </div>
</template>

<script   lang="ts">
import { ref, defineComponent } from 'vue'
export default defineComponent({
    name: 'Home',
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