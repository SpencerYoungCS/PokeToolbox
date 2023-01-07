<script>
export default {
    data() {
        return {
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
            }
        }
    },
    methods: {
        getTypeClass(typeName) {
            return `type type-${typeName.toLowerCase()}`;
        },
        getEffClass(typeEff) {
            const eff = {
                "0": "immune",
                "0.5": "noteffective",
                "1": "normal",
                "2": "veryeffective"
            };

            return `eff eff-${eff[typeEff]}`;
        }
    }
};

</script>

<template>
    <h1 style="text-align:center">Pokemon Type Chart</h1>
    <div style="display: flex; justify-content: center;">
        <table class="table table-sm table-bordered">
            <thead>
                <tr>
                    <th>Types</th>
                    <th v-for="(type, typeName) in types" :class="getTypeClass(typeName)"> {{ typeName }}</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(type, typeName) in types">
                    <th :class="getTypeClass(typeName)">{{ typeName }}</th>
                    <td v-for="(vsTypeEff, vsTypeName) in type" :class="getEffClass(vsTypeEff)">{{ vsTypeEff }}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<style lang="scss">
$color-bug: #a8b820;
$color-dark: #705848;
$color-dragon: #7038f8;
$color-electric: #f8d030;
$color-fairy: #ee99ac;
$color-fighting: #c03028;
$color-fire: #f08030;
$color-flying: #a890f0;
$color-ghost: #705898;
$color-grass: #78c850;
$color-ground: #e0c068;
$color-ice: #98d8d8;
$color-normal: #a8a878;
$color-poison: #a040a0;
$color-psychic: #f85888;
$color-rock: #b8a038;
$color-steel: #b8b8d0;
$color-water: #6890f0;
$color-eff-immune: #525252;
$color-eff-noteffective: #470a0a;
$color-eff-veryeffective:#032b03;
$field-width: 35px;

@mixin type($color) {
  background-color: $color;
  border-color: $color;
}

body {
}

h1 {
  margin: 0.5em 0;
}

.table {
  td,th {
    color: white;
    text-align: center;
    border-color:$color-eff-immune;
    border-collapse: collapse;
    border-style: solid;
    border-width: 0px;
    border-bottom-width: 1px;
    border-right-width: 1px;
  }
  thead th {
    border-bottom-width: 1px;
  }

  .eff {
    &-immune {
      background-color: $color-eff-immune;
    }
    &-veryeffective {
      background-color: $color-eff-veryeffective;
    }
    &-noteffective {
      background-color: $color-eff-noteffective;
    }
  }

  .type {
    color: #fff;
    text-shadow:0 0 8px rgba(93, 93, 93, 0.39);
    &-bug {
      @include type($color-bug);
    }
    &-dragon {
      @include type($color-bug);
    }
    &-dark {
      @include type($color-dark);
    }
    &-dragon {
      @include type($color-dragon);
    }
    &-electric {
      @include type($color-electric);
    }
    &-fairy {
      @include type($color-fairy);
    }
    &-fighting {
      @include type($color-fighting);
    }
    &-fire {
      @include type($color-fire);
    }
    &-flying {
      @include type($color-flying);
    }
    &-ghost {
      @include type($color-ghost);
    }
    &-grass {
      @include type($color-grass);
    }
    &-ground {
      @include type($color-ground);
    }
    &-ice {
      @include type($color-ice);
    }
    &-normal {
      @include type($color-normal);
    }
    &-poison {
      @include type($color-poison);
    }
    &-psychic {
      @include type($color-psychic);
    }
    &-rock {
      @include type($color-rock);
    }
    &-steel {
      @include type($color-steel);
    }
    &-water {
      @include type($color-water);
    }
  }
}
</style>

