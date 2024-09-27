<template>
    <div class="flex md:px-3 py-3">
        <div class="max-w-sm md:max-w-md rounded overflow-hidden shadow-lg bg-white  ">
            <div class="flex items-center  px-4 pt-4">
                <img class="w-5/12 md:h-36 h-30 object-contain" :src="plan.image" alt="Plan Image">
                <h1 class="mx-4 text-4xl font-medium">+</h1> <!-- Añadido margen para separar el signo "+" de las imágenes -->
                <img class="w-5/12 md:h-36 h-30 object-contain" :src="plan.image2" alt="Plan Image">
            </div>
        
            <div class="min-w-80  md:min-w-96 px-6 py-2   text-center">
                <div class="font-bold  sm:text-xl  md:text-1xl  ">{{ plan.message }}</div>
                <div class="    pb-2 font-bold sm:text-sm  md:text-2xl" style="color: var(--color-app);">${{ plan.price
                }}/MES</div>
                <div class="font-semibold sm:text-sm  md:text-1xl mb-2 pb-5 text-gray-600">{{ plan.window }}</div>

                <button class=" bg-[var(--color-app)] text-white font-bold py-2 px-6 rounded-full hover:bg-opacity-80">
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