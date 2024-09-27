<template>
    <section class="relative py-10 overflow-hidden bg-black sm:py-16 lg:py-24 xl:py-32">
        <div class="absolute inset-0">
            <img class="w-full h-full object-cover" src="/src/images/Cinema_Banner.jpg" alt="" />
        </div>
    
        <div class="absolute inset-0 hidden bg-gradient-to-r md:block from-black to-transparent"></div>
        <div class="absolute inset-0 block bg-black/60 md:hidden"></div>
    
        <div class="relative px-4 mx-auto sm:px-6 lg:px-8 w-full">  
            <div class="text-center mx-auto w-full"> <!-- Cambié el ancho interno a "w-full" -->
                <h2 class="text-3xl font-bold leading-tight text-white sm:text-4xl lg:text-5xl xl:text-6xl">
                    Tu mundo de Entrenimiento
                </h2>
                <hr class="border-t-4   w-2/5 mx-auto my-4" style="border-color: var(--color-app);"/>
                <p class="text-3xl font-medium leading-tight text-white sm:text-3xl lg:text-3xl pt-5">
                    Distribuidor Oficial
                </p>

            </div>
        </div>   
    </section>
    <div class="w-full bg-black text-center">
            <h1 class="text-white p-8 font-medium">Pantallas originales, sin caídas y garantizadas, tienen una duración de 27 días.</h1>
    </div>
</template>
<script>
export default{
    name:'content_1'
}
</script>