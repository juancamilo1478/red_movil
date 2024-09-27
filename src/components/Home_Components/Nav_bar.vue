<template>
   
    <header class="lg:px-16 px-4 bg-white flex flex-wrap items-center py-4 shadow-md">
        
        <div class="flex-1 flex justify-between items-center">
            <img src="/src/images/LOGO REDMOVIL.png" alt="image" class="max-w-[200px]" />
          
        </div>
        <label for="menu-toggle" class="pointer-cursor md:hidden block" @click="toggleMenu">
          <svg class="fill-current text-gray-950"
            xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 20 20">
            <title>menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path>
          </svg>
        </label>
        <input class="hidden" type="checkbox" id="menu-toggle" />
         <!-- Overlay -->
         <div v-if="menuOpen" class="fixed inset-0 bg-black opacity-95 z-40 text-white font-bold flex items-center justify-center " @click="toggleMenu">
            <ul class="flex flex-col items-center "> <!-- Utilizar flex-col para centrar verticalmente -->
                <li class="mb-4"><a class="md:p-4 py-3 px-0 block text-5xl sm:text-3xl"  >Productos</a></li>
                <li class="mb-4"><a class="md:p-4 py-3 px-0 block text-5xl sm:text-3xl"  >Video ayudas</a></li>
                <li class="mb-4"><a class="md:p-4 py-3 px-0 block text-5xl sm:text-3xl" >Contacto</a></li>
                <li><a class="md:p-4 py-3 px-0 block text-5xl sm:text-3xl" href="#">Soy proveedor</a></li>
            </ul>
        </div>
        <div class="hidden md:flex md:items-center md:w-auto w-full" id="menu">
            <nav>
                <ul class="md:flex items-center justify-between text-base text-gray-700 pt-4 md:pt-0 ">
                    <li><a class="md:p-4 py-3 px-0 font-semibold  " href="#">Productos</a></li>
                    <li><a class="md:p-4 py-3 px-0 font-semibold" href="#">Video ayudas</a></li>
                    <li><a class="md:p-4 py-3 px-0 font-semibold" href="#">Contacto</a></li>
                    <li><a class="md:p-4 py-3 px-0 font-semibold md:mb-0 mb-2" href="#">Soy provedor</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>
 
export default {
    name:'Nav_bar',
    data() {
        return {
            menuOpen: false // Estado para controlar la visibilidad del menú
        };
    },
    methods: {
        toggleMenu() {
            this.menuOpen = !this.menuOpen; // Alternar el estado del menú
        }
    }
}
</script>