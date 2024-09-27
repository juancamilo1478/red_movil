<template>
    <div style="width: 100%;">
        <Nav_bar/>
        <Promotion/>
        <Content_1/>
        <Content_2/>
    </div>
</template>
<script>
import Nav_bar from '@/components/Home_Components/Nav_bar.vue';
import Promotion from '@/components/Home_Components/Promotion.vue';
import Content_1 from '@/components/Home_Components/Content_1.vue';
import Content_2 from '@/components/Home_Components/Content_2.vue';
export default {
    name: 'Home',
    components: {
    Nav_bar,
    Promotion,
    Content_1,
    Content_2
  },
}
</script>