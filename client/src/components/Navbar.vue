<template>
    <div class="header">
        <div class="navbar-top container-fluid">
            <div class="row">
                <div class="col-12 col-md-4 text-center">
                    <a href="#" class="navbar-brand">
                        <img
                            style="width: 50%"
                            src="../assets/logo.png"
                            alt="pefra-logo"
                            id="navbar-brand_image"
                        />
                    </a>
                </div>
                <div class="col-12 col-md-4"></div>
                <div class="col-12 col-md-4 text-center">
                    <i class="fab fa-facebook-square nav-icons"></i>
                    <i class="fab fa-instagram nav-icons"></i>
                </div>
            </div>
        </div>
        <div class="navbar-bottom">
            <nav class="navbar navbar-expand-md navbar-dark pefra-primary">
                <div class="container">
                    <button
                        class="navbar-toggler"
                        type="button"
                        data-toggle="collapse"
                        data-target="#navbar10"
                    >
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    <div class="navbar-collapse collapse" id="navbar10">
                        <ul class="navbar-nav nav-fill w-100">
                            <li class="nav-item">
                                <a class="nav-link mr-4 mt-2 mb-2" href="#"
                                    >Link</a
                                >
                            </li>
                            <li class="nav-item">
                                <a
                                    class="nav-link mr-4 mt-2 mb-2"
                                    href="//codeply.com"
                                    >Codeply</a
                                >
                            </li>
                            <li class="nav-item">
                                <a class="nav-link mr-4 mt-2 mb-2" href="#"
                                    >Link</a
                                >
                            </li>
                            <li class="nav-item">
                                <a class="nav-link mr-4 mt-2 mb-2" href="#"
                                    >Link</a
                                >
                            </li>
                            <li class="nav-item">
                                <a class="nav-link mr-4 mt-2 mb-2" href="#"
                                    >Link</a
                                >
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        isEditable: Boolean,
    },

    data() {
        return {
            navIsCollapsed: false,
        };
    },
    methods: {
        toggleNav() {
            this.navIsCollapsed = !this.navIsCollapsed;
        },
    },
};
</script>

<style>
.nav-icons {
    font-size: 50px;
    color: #2b77b5;
    display: inline-block;
}

.abs-center-x {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
}

.pefra-primary {
    background-color: #2b77b5;
}

.nav-link {
    color: #2b77b5 !important;
    background-color: white;
    border-radius: 50px;
}
</style>