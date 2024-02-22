<template>
    <div class="layout">
        <div class="Dimension-Title">
            <div>Basic Map Representation</div>
        </div>

        <div class="Dimension-Border">
            <div class="Dimension-Layout">
                <div class="element" id="Political-Map">
                    Political Map
                    <div class="img"><img src="../assets/PoliticalMap.svg" /></div>
                </div>

                <div class="element" id="Shape-based-Map">
                    Shape-based Map
                    <div class="img"><img src="../assets/Shape-basedMap.svg" /></div>
                </div>

                <div class="element" id="Grid-Cartogram">
                    Grid Cartogram
                    <div class="img"><img src="../assets/GridCartogram.svg" /></div>
                </div>

                <div class="element" id="Topographic-Map">
                    Topographic Map
                    <div class="img"><img src="../assets/TopographicMap.svg" /></div>
                </div>

                <div class="element" id="Street-Map">
                    Street Map
                    <div class="img"><img src="../assets/StreetMap.svg" /></div>
                </div>
            </div>
        </div>

    </div>
</template>
    
<script>

</script>
    
<style scoped>
.Dimension-Border {
    border-color: #A9B8C6;
}

.Dimension-Title {
    background-color: #A9B8C6;
}

#Political-Map {
    grid-column: 1 / 2;
}

#Shape-based-Map {
    grid-column: 2 / 3;
}

#Grid-Cartogram {
    grid-column: 3 / 4;
}

#Topographic-Map {
    grid-column: 4 / 5;
}

#Street-Map {
    grid-column: 5 / 6;
}
</style>
    