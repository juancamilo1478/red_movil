<template>
    <div class="flex md:px-3 py-3">
        <div class="max-w-sm md:max-w-md rounded overflow-hidden   bg-white  py-2  pt-6" style="box-shadow: 0 4px 15px rgba(0, 0, 0, 0.151);">
            <div class="flex items-center justify-center w-full">
                <img class="w-2/12 md:h-36 h-30 object-contain" :src="plan.image" alt="Plan Image">
                <h1 class="mx-4 text-4xl font-medium">+</h1> <!-- Añadido margen para separar el signo "+" de las imágenes -->
                <img class="w-2/12 md:h-36 h-30 object-contain" :src="plan.image2" alt="Plan Image">
                <h1 class="mx-4 text-4xl font-medium">+</h1> <!-- Añadido margen para separar el signo "+" de las imágenes -->
                <img class="w-2/12 md:h-36 h-30 object-contain" :src="plan.image2" alt="Plan Image">
            </div>
        
            <div class="min-w-72  md:min-w-72 px-1 py-2   text-center">
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
export default{
    name:"promotions",
    props: {
        plan: {
            type: Object,
            required: true,
        }
    }
}
</script>