<template>
    <section class="w-full py-6">
        <div class="w-10/12 md:w-3/4 mx-auto  ">
            <div class="inline-block pt-11">
                <h2 class="text-2xl font-bold whitespace-nowrap md:text-4xl">Cuentas Individuales</h2>
                <hr class="border-t-4   w-full mt-4" style="border-color: var(--color-app);"  />
                <h2 class="text-1xl font-semibold whitespace-nowrap pt-2">Las visibles tienen stock</h2>
            </div>
        </div>
        <div class="flex flex-wrap justify-center w-3/4 mx-auto pt-8">
            <Cards_services  v-for="(plan, index) in plans"  :key="index" 
            :plan="plan"/>

        </div>
    </section>
    
    <section class="w-full" style="background:var(--color-app)">
        <div class="w-3/4 mx-auto  ">
            <div class="inline-block pt-11 text-white ">
                <h2 class="text-4xl font-bold whitespace-nowrap" >Cuentas Duos +</h2>
                <hr class="border-t-4   w-full mt-4" style="border-color: white;"  />
                <h2 class="text-1xl font-semibold whitespace-nowrap pt-2">Promociones duos</h2>
            </div>
        </div>
        <div class="w-3/4 mx-auto pt-11">
        <div class="  flex flex-wrap justify-center   mx-auto pt-8" >
            <Card_service_duo  v-for="(duo, index) in duo"  :key="index" 
            :plan="duo"/>
        </div>
    </div>
    </section>
</template>
<script>
import Cards_services from '../Cards/Cards_services.vue';
import Card_service_duo from '../Cards/Card_service_duo.vue';
export default {
    name: 'content_2',
    components:{
        Cards_services,
        Card_service_duo
    },
    data() {
        return {
            plans: [
                { message: 'Disney+ sin canales', window:"(1 pantalla)" , price:"25.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/dvmwf3nwngkrc2rfwsue.png"},
                { message: 'Netflix internacional', window:"(1 pantalla)" , price:"25.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/u5w0iysd5adwvprqqzui.png"},
                { message: 'Paramount+', window:"(1 pantalla)" , price:"5.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421416/a7ytlaycohe6x37vzgzp.png"},
                { message: 'Prime Video', window:"(1 pantalla)" , price:"25.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/rlc6yyqrprenkuzwdemk.png"},
                { message: 'Prime Video', window:"(3 pantalla)" , price:"33.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/rlc6yyqrprenkuzwdemk.png"},
                // Agrega más títulos según sea necesario
            ],
            duo:[
                { message: 'Disney+ & Netflix', window:"(1 pantalla)" , price:"30.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/dvmwf3nwngkrc2rfwsue.png",image2:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/u5w0iysd5adwvprqqzui.png"},
                { message: 'Disney & Paramount', window:"(1 pantalla)" , price:"45.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421416/a7ytlaycohe6x37vzgzp.png",image2:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/dvmwf3nwngkrc2rfwsue.png"},
                { message: 'Netflix & Amazon', window:"(3 pantalla)" , price:"24.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/u5w0iysd5adwvprqqzui.png",image2:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/rlc6yyqrprenkuzwdemk.png"},
                { message: 'Disney & Amazon', window:"(1 pantalla)" , price:"17.000" ,image:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/dvmwf3nwngkrc2rfwsue.png",image2:"https://res.cloudinary.com/dirsusbyy/image/upload/v1727421135/rlc6yyqrprenkuzwdemk.png"},
                
            ]
        }
    }
}
</script>