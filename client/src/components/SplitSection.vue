<template>
    <div class="split-section pt-5">
        <div class="container">
            <div class="row">
                <div class="col-12 col-md-6">
                    <h1 class="text-center" style="color: #2b77b5">
                        Kde nás najdete
                    </h1>
                    <div
                        id="map-container-google-1"
                        class="z-depth-1-half map-container"
                        style="height: 500px"
                    >
                        <iframe
                            src="https://maps.google.com/maps?q=manhatan&t=&z=13&ie=UTF8&iwloc=&output=embed"
                            frameborder="0"
                            style="border: 0"
                            allowfullscreen
                        ></iframe>
                    </div>
                </div>
                <div class="col-12 col-md-6 about-us">
                    <p id="about-text">
                        Lorem ipsum lorem ipsum lorem ipsum lorem ipsum lorem
                        ipsum
                    </p>
                    <a id="about-button">Více o nás</a>
                    <img
                        src="../assets/service_1.jpg"
                        class="img-fluid"
                        id="image-about"
                        alt=""
                    />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style>
.about-us {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 0px;
}

#image-about {
    width: 100%;
}

.map-container {
    overflow: hidden;
    padding-bottom: 56.25%;
    position: relative;
    height: 0;
}
.map-container iframe {
    left: 0;
    top: 0;
    height: 100%;
    width: 100%;
    position: absolute;
}

#about-text {
    position: absolute;
    color: white;
    font-size: 25px;
    max-width: 80%;
    top: 70%;
}

#about-button {
    position: absolute;
    left: 70%;
    top: 82%;
    background-color: #2b77b5;
    border-radius: 10px;
    border-color: none;
    outline: none;
    box-shadow: none;
    padding: 15px;
    color: white;
}
</style>