<template>
    <div class="home">
        <Navbar :isEditable="false" />
        <Carousel />
        <Services />
        <ServiceCover />
        <SplitSection />
        <Paralax />
        <Footer />
    </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Carousel from "@/components/Carousel.vue";
import Services from "@/components/Services.vue";
import ServiceCover from "@/components/ServiceCover.vue";
import SplitSection from "@/components/SplitSection.vue";
import Paralax from "@/components/Paralax.vue";
import Footer from "@/components/Footer.vue";

export default {
    name: "Home",
    components: {
        Navbar,
        Carousel,
        Services,
        ServiceCover,
        SplitSection,
        Paralax,
        Footer,
    },

    created() {
        console.log(this.$route);
    },
};
</script>
