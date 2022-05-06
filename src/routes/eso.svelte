<script>
    import { skipTracing } from './eso/skipTracing.js';//This is the info for each table
    import { debtorPayment } from './eso/DebtorPayment.js';
    import { debtorContactEnh } from './eso/DebtorContactEnh.js';
    import { infoDataManag } from './eso/infoDataManag.js';
    import { clientAccess } from './eso/ClientAccess.js';
    import { speci } from './eso/Speci.js';
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

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each debtorPayment as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> <br> <h2>Debtor Contact Enhancements:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each debtorContactEnh as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> <br> <h2>Information & Data Management:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each infoDataManag as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> <br> <h2>Client Access:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each clientAccess as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> <br> <h2>Specialization:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each speci as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}



<!--this is where the acc ends-->

<footer>
    <p>
        information and stuff with things
    </p>
</footer>
<style lang="scss">
    @import 'styles/components';

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