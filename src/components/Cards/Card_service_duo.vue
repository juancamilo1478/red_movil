<template>
    <div class="flex px-3 py-3">
        <div class="max-w-sm md:max-w-md rounded overflow-hidden shadow-lg bg-white  ">
            <div class="flex items-center  px-4">
                <img class="w-5/12 h-52 object-contain" :src="plan.image" alt="Plan Image">
                <h1 class="mx-4 text-4xl font-medium">+</h1> <!-- Añadido margen para separar el signo "+" de las imágenes -->
                <img class="w-5/12 h-52 object-contain" :src="plan.image2" alt="Plan Image">
            </div>
        
            <div class="min-w-96 px-6 py-4   text-center">
                <div class="font-bold text-xl mb-2">{{ plan.message }}</div>
                <div class="font-bold text-xl mb-2 pb-7">{{ plan.window }}</div>
                <button class="bg-[var(--color-app)] text-white font-bold py-2 px-6 rounded-full hover:bg-opacity-80">
                    Obtener Ahora
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'Card_services_duo',
    props: {
        plan: {
            type: Object,
            required: true,
        }
    }
}
</script>