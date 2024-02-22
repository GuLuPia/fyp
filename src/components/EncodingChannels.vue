<template>
    <div class="layout">

        <div class="Dimension-Title">
            <div>Encoding Channels</div>
        </div>

        <div class="Dimension-Border">
            <div class="Dimension-Layout">
                <div class="element" id="Color-Luminance">
                    Color(Luminance)
                    <div class="img"><img src="../assets/Color(Luminance).svg" /></div>
                </div>

                <div class="element" id="3D-Length">
                    3D Length
                    <div class="img"><img src="../assets/3DLength.svg" /></div>
                </div>

                <div class="element" id="Link-Line">
                    Link(Line)
                    <div class="img"><img src="../assets/Link(Line).svg" /></div>
                </div>

                <div class="element" id="Size">
                    Size
                    <div class="img"><img src="../assets/Size.svg" /></div>
                </div>

                <div class="element" id="Color-Hue">
                    Color(Hue)
                    <div class="img"><img src="../assets/Color(Hue).svg" /></div>
                </div>

                <div class="element" id="Glyph">
                    Glyph
                    <div class="img"><img src="../assets/3DLength.svg" /></div>
                </div>

                <div class="element" id="Link-Arrow">
                    Link(Arrow)
                    <div class="img"><img src="../assets/Link(Arrow).svg" /></div>
                </div>

                <div class="element" id="Quantity">
                    Quantity
                    <div class="img"><img src="../assets/Quantity.svg" /></div>
                </div>
            </div>
        </div>


    </div>
</template>
    
<script>

</script>
    
<style scoped>
.Dimension-Border {
    border-color: #C2C531;
}

.Dimension-Title {
    background-color: #C2C531;
}

#Color-Luminance{
    grid-row: 1 / 2;
    grid-column: 1 / 2;
}

#3D-Length{
    grid-row: 1 / 2;
    grid-column: 2 / 3;
}

#Link-Line{
    grid-row: 1 / 2;
    grid-column: 3 / 4;
}

#Size{
    grid-row: 1 / 2;
    grid-column: 4 / 5;
}

#Color-Hue{
    grid-row: 2 / 3;
    grid-column: 1 / 2;
}

#Glyph{
    grid-row: 2 / 3;
    grid-column: 2 / 3;
}

#Link-Arrow{
    grid-row: 2 / 3;
    grid-column: 3 / 4;
}

#Quantity{
    grid-row: 2 / 3;
    grid-column: 4 / 5;
}
</style>
    