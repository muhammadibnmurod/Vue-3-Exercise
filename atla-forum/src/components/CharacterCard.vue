<script>
export default {
    props: {
        character: {
            type: Object,
            required: true
        }
    },
    emits: ['favorite'],
    methods: {
        favoriteCharacter(character) {
            this.favoriteList.push(character)
        },
    }
}
</script>

<template>
    <div>
        <p>{{ character.name }}</p>
        <button>⭐ Favorite</button>
    </div>
</template>