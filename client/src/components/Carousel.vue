<template>
    <div class="section-carousel">
        <div
            id="carouselExampleIndicators"
            class="carousel slide"
            data-ride="carousel"
        >
            <ol class="carousel-indicators">
                <li
                    data-target="#carouselExampleIndicators"
                    data-slide-to="0"
                    class="active"
                ></li>
                <li
                    data-target="#carouselExampleIndicators"
                    data-slide-to="1"
                ></li>
                <li
                    data-target="#carouselExampleIndicators"
                    data-slide-to="2"
                ></li>
            </ol>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img
                        class="d-block w-100"
                        src="../assets/carousel_1.jpg"
                        alt="First slide"
                    />
                </div>
                <div class="carousel-item">
                    <img
                        class="d-block w-100"
                        src="../assets/carousel_1.jpg"
                        alt="Second slide"
                    />
                </div>
                <div class="carousel-item">
                    <img
                        class="d-block w-100"
                        src="../assets/carousel_1.jpg"
                        alt="Third slide"
                    />
                </div>
            </div>
            <a
                class="carousel-control-prev"
                href="#carouselExampleIndicators"
                role="button"
                data-slide="prev"
            >
                <span
                    class="carousel-control-prev-icon"
                    aria-hidden="true"
                ></span>
                <span class="sr-only">Previous</span>
            </a>
            <a
                class="carousel-control-next"
                href="#carouselExampleIndicators"
                role="button"
                data-slide="next"
            >
                <span
                    class="carousel-control-next-icon"
                    aria-hidden="true"
                ></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
        <img src="../assets/triangle.png" class="img-fluid" id="arrow-img" />
        <h1 id="arrow-text">Jsme nejlepší pičo</h1>
    </div>
</template>

<script>
export default {
    name: "Carousel",
};
</script>

<style>
.section-carousel {
    position: relative;
}

.carousel-item > img {
    max-height: 980px !important;
}

#arrow-img {
    position: absolute;
    bottom: 0%;
    right: 0%;
}

.image-text_box {
    position: absolute;
    right: 5%;
    bottom: 5%;
}

#arrow-text {
    position: absolute;
    right: 7.8%;
    bottom: 25%;
    transform: rotate(-46.7deg);
    color: white;
}
</style>