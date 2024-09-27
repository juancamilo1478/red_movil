<template>
    <div class="flex md:px-3 py-3">
        <div class="max-w-sm rounded overflow-hidden shadow-lg ">
            <img class="w-full md:h-52 h-40  object-cover" :src="plan.image" alt="Plan Image">
            <div class="min-w-96 px-6 py-4 bg-gray-200 text-center">
                <div class="font-bold text-xl mb-2">{{ plan.message }}</div>
                <div class="font-bold text-xl mb-2 pb-7">{{ plan.window }}</div>
                <button class="bg-[var(--color-app)] text-white font-bold py-2 px-6 rounded-full hover:bg-opacity-80">
                    Comprar
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'Card_services',
    props: {
        plan: {
            type: Object,
            required: true,
        }
    }
}
</script>