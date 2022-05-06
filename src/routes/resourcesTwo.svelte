<script>
    import { skipTracing } from './eso/skipTracing.js';//This is the info for each table
    import Accordion from './Accordion.svelte'; //the structure of the accordian
    import MapModal from './MapModal.svelte';//the modal popup in the accordion items

    let continentMap = "";
    let modalShowing = false;

    const showMap = (mapURL) => {
        continentMap = mapURL;
        modalShowing = true;
    }
</script>


<header>
    <h1>Eso</h1>
    <p>Extended service options</p>
    <p>Debt$Net® collection software offers Extended Service Options, or ESOs. Extended Service Options are add-on modules that provide advanced functionality to collection agencies, including those with specific client-driven requirements. These add-on modules allow you to pay for only those features you require, letting Debt$Net® more fully automate your collection operations. Your agency may require none, or only a few of these Extended Service Options, however, for those who want power features, Extended Services options are available.</p>
</header>

<!--this is where the accordion starts-->

<h2>Skip Tracing & Scoring:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each skipTracing as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> <br> <h2>Debtor Payment Capabilities:</h2>




<!--this is where the acc ends-->


<style lang="scss">
    @import 'styles/components';

   header{
       width: 100%;
       text-align: center;
   }


</style>