<template>
    <div class="flex md:px-2 py-3 w-80 ">
        <div class="min-w-xs rounded overflow-hidden    " style="box-shadow: 0 4px 15px rgba(0, 0, 0, 0.151);">
            <div class="flex items-center justify-center  ">
                <img class="w-5/12 object-contain h-36   " :src="plan.image" alt="Plan Image">
            </div>
            <div class="    min-w-xs   py-4 bg-gray-100  text-center">
                <div class="font-bold  sm:text-xl  md:text-1xl  ">{{ plan.message }}</div>
                <div class="    pb-2 font-bold sm:text-sm  md:text-2xl" style="color: var(--color-app);">${{ plan.price
                }}/MES</div>
                <div class="font-semibold sm:text-sm  md:text-1xl mb-2 pb-7 text-gray-600">{{ plan.window }}</div>

                <button class="bg-[var(--color-app)] text-white font-bold py-2 px-6 rounded-full hover:bg-opacity-80">
                    Comprar
                </button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Card_services',
    props: {
        plan: {
            type: Object,
            required: true,
        }
    }
}
</script>