<template>
    <div class="about">
        <h1>This is an about page</h1>
        <Navbar :isEditable="isEditable"></Navbar>
    </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";

export default {
    name: "Home",
    components: {
        Navbar,
    },

    data() {
        return {
            isEditable: false,
        };
    },

    created() {
        if (this.$route.name === "Home") {
            this.isEditable = false;
        } else {
            this.isEditable = true;
        }
    },
};
</script>
