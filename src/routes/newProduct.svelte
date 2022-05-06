<script>
    import { Packs } from './feats/Packs.js';//This is the info for each table
    
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
    <h1>Features or Packages</h1>
    <p>Extended service options</p>
    <p>Debt$Net® collection software offers Extended Service Options, or ESOs. Extended Service Options are add-on modules that provide advanced functionality to collection agencies, including those with specific client-driven requirements. These add-on modules allow you to pay for only those features you require, letting Debt$Net® more fully automate your collection operations. Your agency may require none, or only a few of these Extended Service Options, however, for those who want power features, Extended Services options are available.</p>
</header>

<!--this is where the accordion starts-->

<h2>Packages:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each Packs as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> <br> 


<!--this is where the acc ends-->

<h2>Automated Dunning Notices</h2>

<p>Debt$Net® lets you create more then twelve hundred notices of your own design. The content of a notice is totally free form, letting you set up any kind of notice you need and easily pull information from the Debt$Net® files into your notice. Besides the standard notice variable, you can calculate data and create your own variables, you can chain notices into a series and have multiple dunning notice series as well. Design one dunning series to accommodate medical collections and another for commercial or retail collections. As accounts are processed through the dunning series, you can automatically turn them over to a collector for a call. The dunning series can update the status, priority or collector assigned to the account. They can interrupt the notification sequence, restart, or redirect it at their discretion. Collectors can even print quick notices without interrupting the processing of the dunning series. Debt$Net® can also export notices to outsource companies.</p>


<style lang="scss">
    @import 'styles/components';

   header{
       width: 100%;
       text-align: center;
   }

   

</style>