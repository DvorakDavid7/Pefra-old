<template>
    <div class="cover-section text-center">
        <h1 class="pt-3" id="cover-title">Pokrytí našich služeb</h1>
        <div class="service-cover">
            <div class="diamond" id="diamond-1">
                <div class="cut-diamond"></div>
            </div>
            <div class="diamond" id="diamond-2">
                <div class="cut-diamond"></div>
            </div>
            <div class="diamond" id="diamond-3">
                <div class="cut-diamond"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style>
.cover-section {
    position: relative;
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
}

.service-cover {
    position: absolute;
    transform-origin: 50%;
    top: 15%;
    height: 85%;
    width: 70%;
    background: url("../../src/assets/service_map.jpg");
    background-size: 100%;
    background-repeat: no-repeat;
    z-index: 999;
}

.cover-section {
    background-color: #2b77b5;
}

#cover-title {
    color: white;
}

#cover-img {
    height: 90%;
    width: 20%;
}

/* triangle ----------------------------------------*/
.diamond {
    position: absolute;
    height: 15%;
}

/* triangles instances */
#diamond-1 {
    top: 50%;
    right: 20%;
}

#diamond-2 {
    top: 40%;
    right: 50%;
}

#diamond-3 {
    top: 30%;
    right: 60%;
}

.cut-diamond {
    border-style: solid;
    border-color: transparent transparent #2b77b5 transparent;
    border-width: 0 25px 25px 25px;
    height: 0;
    width: 50px;
    box-sizing: content-box;
    position: relative;
    margin: 20px 0 50px 0;
    z-index: 999;
}
.cut-diamond:after {
    content: "";
    position: absolute;
    top: 25px;
    left: -25px;
    width: 0;
    height: 0;
    border-style: solid;
    border-color: #2b77b5 transparent transparent transparent;
    border-width: 70px 50px 0 50px;
}

.diamond:after {
    content: " ";
    display: block;
    background: #2b77b5;
    height: 80%;
    width: 150%;
    position: absolute;
    z-index: 999;
    left: 95%;
    top: -49%;
    border-radius: 15px;
    display: none;
}

.diamond:hover::after {
    display: block;
}

/* .diamond-text {
    position: absolute;
    background-color: #2b77b5;
    height: 10vh;
    width: 15vh;
    border-radius: 20px;
    z-index: 999;
}

#diamond-title {
    font-size: 18px;
    margin-top: 5px;
    color: white;
}

#diamond-text {
    font-size: 13px;
    color: white;
} */
</style>