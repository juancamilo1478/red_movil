<template>
    <section class="w-full">
        <div class="w-3/4 mx-auto pt-11">
            <div class="inline-block pt-11">
                <h2 class="text-4xl font-bold whitespace-nowrap" >Cuentas Individuales</h2>
                <hr class="border-t-4   w-full mt-4" style="border-color: var(--color-app);"  />
                <h2 class="text-1xl font-semibold whitespace-nowrap pt-2">Las visibles tienen stock</h2>
            </div>
        </div>
        <div class="w-3/4 mx-auto pt-11">
             
        </div>
    </section>
</template>
<script>
export default {
    name: 'content_2',
    data() {
        return {
            plans: [
                { message: 'Disney+ sin canales', window:"(1 pantalla)" , price:"25.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/dvmwf3nwngkrc2rfwsue.png"},
                { message: 'Netflix internacional', window:"(1 pantalla)" , price:"25.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/u5w0iysd5adwvprqqzui.png"},
                { message: 'Paramount+', window:"" , price:"5.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421416/a7ytlaycohe6x37vzgzp.png"},
                { message: 'Prime Video', window:"(1 pantalla)" , price:"25.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/rlc6yyqrprenkuzwdemk.png"},
                { message: 'Prime Video', window:"(3 pantalla)" , price:"33.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/rlc6yyqrprenkuzwdemk.png"},
                // Agrega más títulos según sea necesario
            ]
        }
    }
}
</script>