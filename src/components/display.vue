<template>
    <div class="team"> {{teamName}} </div>
    <div :key= player.id v-for="player in players">
        <h2> {{player.id}} {{player.firstName}} {{player.lastName}} </h2>
        <h3> {{player.country}} </h3>
    </div>
</template>

<script>
export default {
    name: "Display",
    props: {
        teamName: String,
        players: []
    },
    updated() {
        console.log(players);
    }
}
</script>