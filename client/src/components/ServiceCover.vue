<template>
    <div class="cover-section text-center">
        <h1 class="pt-3" id="cover-title">Pokrytí našich služeb</h1>
        <div class="service-cover">
            <img
                src="../assets/services_map.png"
                alt=""
                class="img-fluid mt-2"
                id="cover-img"
            />
        </div>
    </div>
</template>

<script>
export default {};
</script>

<style>
.service-cover {
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
}

.cover-section {
    background-color: #2b77b5;
}

#cover-title {
    color: white;
}

#cover-img {
    height: 90%;
}
</style>