<script>
export default {
    data() {
        return {
            // type: '',
            // fullImageDir: '',
            listOfTypes: 
                [
                    "Normal",
                    "Fire",
                    "Water",
                    "Grass",
                    "Electric",
                    "Ice",
                    "Fighting",
                    "Poison",
                    "Ground",
                    "Flying",
                    "Psychic",
                    "Bug",
                    "Rock",
                    "Ghost",
                    "Dark",
                    "Dragon",
                    "Steel",
                    "Fairy"
                ],
            leftSelected: [],
            rightSelected: [],
            currAdv: 0,
            eachAdv: [],
            types: {
                Bug: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 0.5,
                    Fire: 2,
                    Flying: 2,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 0.5,
                    Ice: 1,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 2,
                    Steel: 1,
                    Water: 1
                },
                Dark: {
                    Bug: 2,
                    Dark: 0.5,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 2,
                    Fighting: 2,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 0.5,
                    Grass: 1,
                    Ground: 1,
                    Ice: 1,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 0,
                    Rock: 1,
                    Steel: 1,
                    Water: 1
                },
                Dragon: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 2,
                    Electric: 0.5,
                    Fairy: 2,
                    Fighting: 1,
                    Fire: 0.5,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 1,
                    Ice: 2,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 1,
                    Water: 0.5
                },
                Electric: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 0.5,
                    Fairy: 1,
                    Fighting: 1,
                    Fire: 1,
                    Flying: 0.5,
                    Ghost: 1,
                    Grass: 1,
                    Ground: 2,
                    Ice: 1,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 0.5,
                    Water: 1
                },
                Fairy: {
                    Bug: 0.5,
                    Dark: 0.5,
                    Dragon: 0,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 0.5,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 1,
                    Ground: 1,
                    Ice: 1,
                    Normal: 1,
                    Poison: 2,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 2,
                    Water: 1
                },
                Fighting: {
                    Bug: 0.5,
                    Dark: 0.5,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 2,
                    Fighting: 1,
                    Fire: 1,
                    Flying: 2,
                    Ghost: 1,
                    Grass: 1,
                    Ground: 1,
                    Ice: 1,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 2,
                    Rock: 0.5,
                    Steel: 1,
                    Water: 1
                },
                Fire: {
                    Bug: 0.5,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 0.5,
                    Fighting: 1,
                    Fire: 0.5,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 2,
                    Ice: 0.5,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 2,
                    Steel: 0.5,
                    Water: 2
                },
                Flying: {
                    Bug: 0.5,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 2,
                    Fairy: 1,
                    Fighting: 0.5,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 0,
                    Ice: 2,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 2,
                    Steel: 1,
                    Water: 1
                },
                Ghost: {
                    Bug: 0.5,
                    Dark: 2,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 0,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 2,
                    Grass: 1,
                    Ground: 1,
                    Ice: 1,
                    Normal: 0,
                    Poison: 0.5,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 1,
                    Water: 1
                },
                Grass: {
                    Bug: 2,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 0.5,
                    Fairy: 1,
                    Fighting: 1,
                    Fire: 2,
                    Flying: 2,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 0.5,
                    Ice: 2,
                    Normal: 1,
                    Poison: 2,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 1,
                    Water: 0.5
                },
                Ground: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 0,
                    Fairy: 1,
                    Fighting: 1,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 2,
                    Ground: 1,
                    Ice: 2,
                    Normal: 1,
                    Poison: 0.5,
                    Psychic: 1,
                    Rock: 0.5,
                    Steel: 1,
                    Water: 2
                },
                Ice: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 2,
                    Fire: 2,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 1,
                    Ground: 1,
                    Ice: 0.5,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 2,
                    Steel: 2,
                    Water: 1
                },
                Normal: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 2,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 0,
                    Grass: 1,
                    Ground: 1,
                    Ice: 1,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 1,
                    Water: 1
                },
                Poison: {
                    Bug: 0.5,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 0.5,
                    Fighting: 0.5,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 2,
                    Ice: 1,
                    Normal: 1,
                    Poison: 0.5,
                    Psychic: 2,
                    Rock: 1,
                    Steel: 1,
                    Water: 1
                },
                Psychic: {
                    Bug: 2,
                    Dark: 2,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 0.5,
                    Fire: 1,
                    Flying: 1,
                    Ghost: 2,
                    Grass: 1,
                    Ground: 1,
                    Ice: 1,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 0.5,
                    Rock: 1,
                    Steel: 1,
                    Water: 1
                },
                Rock: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 1,
                    Fairy: 1,
                    Fighting: 2,
                    Fire: 0.5,
                    Flying: 0.5,
                    Ghost: 1,
                    Grass: 2,
                    Ground: 2,
                    Ice: 1,
                    Normal: 0.5,
                    Poison: 0.5,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 2,
                    Water: 2
                },
                Steel: {
                    Bug: 0.5,
                    Dark: 1,
                    Dragon: 0.5,
                    Electric: 1,
                    Fairy: 0.5,
                    Fighting: 2,
                    Fire: 2,
                    Flying: 0.5,
                    Ghost: 1,
                    Grass: 0.5,
                    Ground: 2,
                    Ice: 0.5,
                    Normal: 0.5,
                    Poison: 0,
                    Psychic: 0.5,
                    Rock: 0.5,
                    Steel: 0.5,
                    Water: 1
                },
                Water: {
                    Bug: 1,
                    Dark: 1,
                    Dragon: 1,
                    Electric: 2,
                    Fairy: 1,
                    Fighting: 1,
                    Fire: 0.5,
                    Flying: 1,
                    Ghost: 1,
                    Grass: 2,
                    Ground: 1,
                    Ice: 0.5,
                    Normal: 1,
                    Poison: 1,
                    Psychic: 1,
                    Rock: 1,
                    Steel: 0.5,
                    Water: 0.5
                }
            },


        };
    },
    methods:
    {
        leftSelect(type)
        {
            // if already exists drop it and recalculate
            const index = this.leftSelected.indexOf(type);
            if(index > -1) 
            {
                const leftItem =  this.leftSelected.splice(index, 1);;
                const refName = `l${leftItem}`;
                this.$refs[refName][0].classList.toggle("highlight", false);
                this.currAdv = this.calculateAdvantage();
                return;
            }

            this.leftSelected.push(type)

            // replace the last one and unhighlight it
            if(this.leftSelected.length > 2)
            {
                const leftItem = this.leftSelected.shift();
                const refName = `l${leftItem}`;
                this.$refs[refName][0].classList.toggle("highlight", false);
            }
            this.currAdv = this.calculateAdvantage();

            const refName = `l${type}`;
            this.$refs[refName][0].classList.toggle("highlight", true);
            // console.log(this.eachAdv)
        },
        rightSelect(type)
        {
            // repeat logic from left side
            const index = this.rightSelected.indexOf(type);
            if(index > -1) 
            {
                const rightItem =  this.rightSelected.splice(index, 1);;
                const refName = `r${rightItem}`;
                this.$refs[refName][0].classList.toggle("highlight", false);
                this.currAdv = this.calculateAdvantage();
                return;
            }

            this.rightSelected.push(type)
            if(this.rightSelected.length > 2) 
            {
                const rightItem = this.rightSelected.shift();
                const refName = `r${rightItem}`;
                this.$refs[refName][0].classList.toggle("highlight", false);
            }
            this.currAdv = this.calculateAdvantage();

            const refName = `r${type}`;
            this.$refs[refName][0].classList.toggle("highlight", true);
            // console.log(this.eachAdv)
        },
        calculateAdvantage()
        {
            this.eachAdv = []
            let adv = 1.0;
            // get values from left and right selected
            for(const rightItem of this.rightSelected)
            {
                for(const leftItem of this.leftSelected)
                {
                    if(this.types[rightItem][leftItem] == 1)  this.eachAdv.push({type: leftItem, vs: rightItem, effectiveness: 'Neutral', rawvalue: this.types[rightItem][leftItem]})
                    if(this.types[rightItem][leftItem] < 1)  this.eachAdv.push({type: leftItem, vs: rightItem, effectiveness: 'Weak', rawvalue: this.types[rightItem][leftItem]})
                    if(this.types[rightItem][leftItem] > 1)  this.eachAdv.push({type: leftItem, vs: rightItem, effectiveness: 'Super Effective', rawvalue: this.types[rightItem][leftItem]})
                   
                    adv *= this.types[rightItem][leftItem]
                }
            }
            return adv;
        },
    },
    mounted()
    {
    },
}

</script>

<template>
    <!-- <div style="width: 100%">?</div> -->
    <div class="container">
        <div class="left-column">
            <div v-for="item in listOfTypes" style="float:left; width: 25%;padding: 5px">
                <img class='iconImg' @click="leftSelect(item)" :ref="'l'+item" :src="`src/assets/typeicons/pokemon_type_icon_${item}.svg`">
            </div>
        </div>
        <div class="middle-column">
            <div class="rows">
                <div class="cols">
                    <div v-for="leftItem in leftSelected" style="width: 80%;padding: 5px">
                        <img @click="leftSelect(leftItem)" :ref="'l'+leftItem"
                            :src="`src/assets/typeicons/pokemon_type_icon_${leftItem}.svg`">
                    </div>
                    <div style="text-align:center"> vs </div>
                    <div v-for="rightItem in rightSelected" style="width: 80%;padding: 5px">
                        <img @click="rightSelect(rightItem)" :ref="'r'+rightItem"
                            :src="`src/assets/typeicons/pokemon_type_icon_${rightItem}.svg`">
                    </div>
                </div>

                <div v-for="row in eachAdv">
                    {{ row['type'] }} is {{ row['effectiveness'] }} agianst {{ row['vs'] }}
                </div>
                <div>
                    Overall: {{ currAdv }}
                </div>
            </div>
    
        </div>
        <div class="right-column">
            <div v-for="item in listOfTypes" style="float:left; width: 25%; padding: 5px">
                <img class='iconImg' @click="rightSelect(item)" :ref="'r'+item" :src="`src/assets/typeicons/pokemon_type_icon_${item}.svg`">
            </div>
        </div>
    
    </div>
        <!-- <button>open typechart</button> -->

</template>

<style scoped>

.container 
{
    display: flex;
}

.left-column
{
    width: 30%;
}
.middle-column
{
    width: 40%;
    padding: 6%;
    display: flex;
    flex-direction: row;
    align-items: top;
    justify-content: center;
    margin-top: 20px;
    
}
.middle-column div
{
    width: 100%;
}

.rows
{
    display: flex;
    flex-direction: column;
    align-items: top;
    justify-content: center;
    width: 100%;
}
.cols
{
    display: flex;
    flex-direction: row;
    align-items: top;
    justify-content: center;
    width: 100%;
}
.right-column
{
    width: 30%;
}
img 
{
    outline: none;
}
img.highlight
{
    outline:2px solid rgb(0, 255, 115)
}
</style>
