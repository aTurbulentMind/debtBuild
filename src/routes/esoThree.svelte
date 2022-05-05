<script>
    import { continents } from './continentsData.js';
    import Continent from './Continent.svelte';
    import MapModal from './MapModal.svelte';

    let continentMap = "";
    let modalShowing = false;

    const showMap = (mapURL) => {
        continentMap = mapURL;
        modalShowing = true;
    }
</script>

<header>
    <h1>The accordion</h1>
    <p>Packin info into stuff</p>
</header>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each continents as {heading, content, learnurl, mapurl}}
<Continent {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<footer>
    <p>
        information and stuff with things
    </p>
</footer>
<style>
   header{
       width: 100%;
       text-align: center;
       color: #8c3420;
   }

   footer{
       width: 100%;
       text-align: right;
       font-size: .8rem;
   }

</style>