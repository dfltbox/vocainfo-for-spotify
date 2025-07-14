<script lang="ts">
    let spotifyLink: string = '';

    function search() {
        //stuff
    }
</script>

<div class="center-container">
    <h1>VocaInfo for <span class="spotify">Spotify</span></h1>
    <p>Simply paste the spotify link below to get all it's <a href="https://vocadb.net" target="_blank">vocadb.net</a> info!</p>
    <div class="input-container">
        <input type="text" bind:value={spotifyLink} placeholder="Paste Spotify link here..." />
        <button on:click={search}>Search</button>
    </div>
</div>

<style>
@import url('https://fonts.googleapis.com/css2?family=TikTok+Sans:opsz,wght@12..36,300..900&display=swap');    

:global(body) {
    font-family: "TikTok Sans", sans-serif;
    background-color: #1f2421;
    color: white;
    margin: 0;
    min-height: 100vh;
}

.center-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 15px;
    margin-top: 10px;
}

.input-container {
    display: flex;
    gap: 0.5rem;
    width: 100%;
    max-width: 700px;
}

.spotify {
    color: #76C893;
}

a {
    color: #168AAD;
    text-decoration: none;
    font-weight: bold;
}

input, button {
    padding: 10px 16px;
    border-radius: 5px;
    font-size: 1rem;
    height: 44px;
    box-sizing: border-box;
}

input {
    background-color: #343a40;
    color: white;
    border: 3px solid #6c757d;
    width: 50%;
    box-shadow: none;
    flex: 1;
}

button {
    border: none;
    background-color: #76C893;
    color: white;
    font-weight: bold;
    cursor: pointer;
}
</style>