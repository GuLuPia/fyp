<template>
    <div class="layout">
        <div class="Dimension-Title">
            <div>Label Positions</div>
        </div>

        <div class="Dimension-Border">
            <div class="Dimension-Layout">
                <div id="Situated">
                    <div class="sub-Title">
                        <div>Situated</div>
                    </div>
                    <div class="sub-Border">
                        <div class="element">
                            <div class="img"><img src="../assets/Situated.svg" /></div>
                        </div>
                    </div>
                </div>

                <div id="Matched">
                    <div class="sub-Title">
                        <div>Matched</div>
                    </div>

                    <div class="sub-Border">
                        <div class="element">
                            Text
                            <div class="img"><img src="../assets/MatchedText.svg" /></div>
                        </div>
                        <div class="element">
                            Icon
                            <div class="img"><img src="../assets/MatchedIcon.svg" /></div>
                        </div>
                        <div class="element">
                            Color
                            <div class="img"><img src="../assets/MathchedColor.svg" /></div>
                        </div>

                    </div>
                </div>

                <div id="Linked">
                    <div class="sub-Title">
                        <div>Linked</div>
                    </div>

                    <div class="sub-Border">
                        <div class="element">
                            Convenient
                            <div class="img"><img src="../assets/LinkedConvenient.svg" /></div>
                        </div>
                        <div class="element">
                            Aligned
                            <div class="img"><img src="../assets/LinkedAligned.svg" /></div>
                        </div>
                        <div class="element">
                            Ordered
                            <div class="img"><img src="../assets/LinkedOrdered.svg" /></div>
                        </div>
                    </div>
                </div>
            </div>

        </div>

    </div>
</template>
    
<script>

</script>
    
<style scoped>
.Dimension-Border {
    border-color: #C497B2;
}

.Dimension-Title {
    background-color: #C497B2;
}

.sub-Title {
    margin-top: 6px;
    padding: 3px;
    font-size: 14px;
    border-radius: 6px;
    display: block;
    width: fit-content;
    background-color: #E1CBD8;
}

.sub-Border {

    clear: both;
    /* border: 2px solid;  */
    border: 1px dotted;
    border-color: #E1CBD8;
    /* display: inline-block;  */

    display: flex;
    flex-direction: column;;
}

#Situated {
    grid-row: 1 / 2;
    grid-column: 1 / 2;
}

#Matched {
    grid-row: 2 / 3;
    grid-column: 1 / 2;
}

#Linked {
    grid-row: 1 / 3;
    grid-column: 2 / 3;
}
</style>    