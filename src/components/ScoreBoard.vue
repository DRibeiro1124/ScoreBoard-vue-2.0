<template>
    <div>
        <header>
            <h1>NBA Score Board</h1>
        </header>
        <section class="main-box">
            <div class="home-team">
            <p>Home Team</p>
            <h3>{{team1DisplayName}}</h3>
            <p class="score">{{team1_score}}</p>
            <div>
                <input v-model="team1Name" type="text" placeholder="Update Home Team Name">
                <button v-on:click="t1_update_name">Update</button>
            </div>
            <div>
                <p>Update Home Team Score</p>
                <button v-on:click="homeTeamAdd1">Add 1</button>  
                <button v-on:click="homeTeamAdd2">Add 2</button>  
                <button v-on:click="homeTeamAdd3">Add 3</button>  
                <button v-on:click="homeTeamSubtract1">Subtract 1</button>  
            </div>
            </div>
            <div class="away-team">
            <p>Away Team</p>
            <h3>{{team2DisplayName}}</h3>
            <p class="score">{{team2_score}}</p>
            <div>
                <input v-model="team2Name" type="text" placeholder="Update Away Team Name">
                <button v-on:click="t2_update_name">Update</button>
            </div>
            <div>
                <p>Update Away Team Score</p>
                <button v-on:click="awayTeamAdd1">Add 1</button>  
                <button v-on:click="awayTeamAdd2">Add 2</button>  
                <button v-on:click="awayTeamAdd3">Add 3</button>  
                <button v-on:click="awayTeamSubtract1">Subtract 1</button>  
            </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: "ScoreBoard",
    data: function () {
        return {
            team1Name: "",
            team2Name: "",
            team1DisplayName: "",
            team2DisplayName: "",
            t1_counter: 0,
            t2_counter: 0,
            team1_score: 0,
            team2_score: 0,

        }
    },
    methods: {
        t1_update_name: function () {
            console.log("updated")
            this.team1DisplayName = this.team1Name
        },

        homeTeamAdd1: function () {
            console.log("add one is being clicked")
            this.team1_score++;
        },

        homeTeamAdd2: function () {
            console.log("add two")
            this.team1_score += 2;
        },

        homeTeamAdd3: function () {
            console.log("add 3")
            this.team1_score += 3;
        },

        homeTeamSubtract1: function () {
            console.log("take one away")
            this.team1_score --;
        },

        t2_update_name: function () {
            console.log("updated")
            this.team2DisplayName = this.team2Name
        },

        awayTeamAdd1: function () {
            console.log("add one is being clicked")
            this.team2_score++;
        },

        awayTeamAdd2: function () {
            console.log("add two")
            this.team2_score += 2;
        },

        awayTeamAdd3: function () {
            console.log("add 3")
            this.team2_score += 3;
        },

        awayTeamSubtract1: function () {
            console.log("take one away")
            this.team2_score --;
        }
        
    }

}
</script>

<style>
    .score {
        font-size: 3em;
    }
</style>
