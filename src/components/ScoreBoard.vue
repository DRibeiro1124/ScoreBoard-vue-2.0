<template>
    <div>
        <header>
            <h1>NBA Score Board</h1>
        </header>
        <section class="main-box">
            <div class="home-team">
                <p>Home Team</p>
                <h3>{{homeTeamDisplayName}}</h3>
                <p class="score">{{homeScore}}</p>
                <div>
                    <input type="text" v-model="homeName" placeholder="Upadate Home Team Name">
                    <button v-on:click="homeTeamUpdateName">Update</button>
                </div>
                <div>
                    <p>Update Home Team Score</p>
                    <button v-on:click="homeTeamAdd1">Add 1</button>

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
                homeName: "",
                homeTeamDisplayName: "Home Team",
                homeScore: 0,
                counter: 0,
            }
        },
        methods: {
            homeTeamUpdateName: function () {
                console.log("home is being updated")
                this.homeTeamDisplayName = this.homeName
            }
        },



    }


</script>

<style>
    .main-box {
        border: 2px solid black;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        height: 25em;
        align-items: center;
        padding: 2em;
    }

    .home-team {
        display: flex;
        flex-direction: column;
    }

    /* .away-team {
        display: flex;
        flex-direction: column;
    } */

    .score {
        font-size: 3em;
    }

    button {
        border: 1px solid black;
        border-radius: 3px;
        padding: 2px;
        margin: 3px;
    }

    button:hover {
        background: blue;
        color: white;
    }
</style>