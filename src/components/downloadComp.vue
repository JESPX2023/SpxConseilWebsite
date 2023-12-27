<template>
    <div id="downloadDiv">
        <a
        id="downloadA"
        href="../assets/brochure/plaquetteSpxConseil.pdf" 
        download
        >
            <button id="downloadButton">
                    <p id="downloadP">
                        {{ $t("download.download") }}
                    </p>
                    <v-icon icon="fas fa-download" />
            </button>
        </a>
    </div>
    <div id="colorBoxDiv">
        <!-- just a colored box -->
    </div>
</template>

<script lang="ts">
export default {

}
</script>

<style scoped>

#downloadDiv {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 10vh;
    margin-bottom: 3vh;
}

#downloadButton {
    display: flex;
    padding: 2vh 4vh;
    font-size: max(1.2vw, 15px);
    font-weight: bold;
    border-radius: 10px;
    box-shadow: 5px 5px 5px rgb(199, 199, 199);
}

#downloadButton:active {
    box-shadow: 1px 1px 5px rgb(199, 199, 199); /* Changement de l'ombre lorsqu'il est cliqué ou en focus */
}

#downloadA {
    display: flex;
    color: black;
    text-decoration: none;
}

#downloadP {
    margin-right: 1vw;
}

#colorBoxDiv {
    height: 6vh;
    background-color: #F3D0D0;
}
</style>