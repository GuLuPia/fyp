<template>
    <div class="layout">
        <div class="Dimension-Title">
            <div>Map Projections</div>
        </div>

        <div class="Dimension-Border">
            <div class="Dimension-Layout">
                <div class="element" id="Mollweide">
                    Mollweide
                    <div class="img"><img src="../assets/Mollweide.svg" /></div>
                </div>

                <div class="element" id="Robinson">
                    Robinson
                    <div class="img"><img src="../assets/Robinson.svg" /></div>
                </div>
            </div>

        </div>

    </div>
</template>
    
<script>

</script>
    
<style scoped>
.Dimension-Border {
    border-color: #96C37D;
}

.Dimension-Title {
    background-color: #96C37D;
}

#Mollweide {
    grid-column: 1 / 2;
}

#Robinson {
    grid-column: 2 / 3;
}
</style>
    