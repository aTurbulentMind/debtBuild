<script>
    import { reso } from './Resources.js';//This is the info for each table
    import Accordion from './components/AccordionTwo.svelte'; //the structure of the accordian
    import MapModal from './components/MapModal.svelte';//the modal popup in the accordion items

    let continentMap = "";
    let modalShowing = false;

    const showMap = (mapURL) => {
        continentMap = mapURL;
        modalShowing = true;
    }
</script>

<body>
    

<header>
    <h1>Affiliates and Requirements</h1>
    <p>Nice words about our awesome partners and affiliates.</p>
    
</header>

<!--this is where the accordion starts-->

<h2>Skip Tracing & Scoring:</h2>

{#if modalShowing}
    <MapModal mapurl={continentMap} on:click={() => modalShowing = false} />
{/if}

{#each reso as {heading, content, learnurl, mapurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
           on:click={() => showMap(mapurl)}/>
{/each}

<!--this is a break--> 




<!--this is where the acc ends-->
<br> <h2>Requirments.</h2>
        <h2>Server:</h2>

<table class="content-table">
    <thead>
        <tr>
            <th>PowerS requirements:</th>
            <th>Minimum</th>
            <th>Recommended</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Windows Operating System</th>
            <th>Windows 7 or Higher</th>
            <th>Server 2008 or Higher</th>
        </tr>
        <tr>
            <th>Processor</th>
            <th>1GHz or Faster</th>
            <th>2 GHz or Faster</th>
        </tr>
        <tr>
            <th>Ram</th>
            <th>8 GB or Higher</th>
            <th>16 GB or Higher</th>
        </tr>
        <tr>
            <th>Free HD Space</th>
            <th>20 GB or More</th>
            <th>40 GB or More</th>
        </tr>
    </tbody>
</table>

<table class="content-table">
    <thead>
        <tr>
            <th>PrestigueS requirements:</th>
            <th>Minimum</th>
            <th>Recommended</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Windows Operating System</th>
            <th>Windows 7 or Higher</th>
            <th>Server 2008 or Higher</th>
        </tr>
        <tr>
            <th>SQL server</th>
            <th>2005 Standard or Newer</th>
            <th>2008 Standard or Newer</th>
        </tr>
        <tr>
            <th>Processor</th>
            <th>1GHz or Faster</th>
            <th>2 GHz or Faster</th>
        </tr>
        <tr>
            <th>Ram</th>
            <th>8 GB or Higher</th>
            <th>16 GB or Higher</th>
        </tr>
        <tr>
            <th>Free HD Space</th>
            <th>20 GB or More</th>
            <th>40 GB or More</th>
        </tr>
    </tbody>
</table>

<h2>Workstations:</h2>

<table class="content-table">
    <thead>
        <tr>
            <th>Requirements:</th>
            <th>Minimum</th>
            <th>Recommended</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th>Windows Operating System</th>
            <th>Windows 7 Professional or Newer</th>
            <th>Windows 7 Professional or Newer</th>
        </tr>
        <tr>
            <th>Processor</th>
            <th>1GHz or Faster</th>
            <th>2 GHz or Faster</th>
        </tr>
        <tr>
            <th>Ram</th>
            <th>2 GB or Higher</th>
            <th>4 GB or Higher</th>
        </tr>
        <tr>
            <th>Free HD Space</th>
            <th>2 GB or More</th>
            <th>5 GB or More</th>
        </tr>
    </tbody>
</table>

</body>
<style lang="scss">
    @import 'styles/components';

   header{
       width: 100%;
       text-align: center;
   }

   .content-table{
       width: 70%;
       border-collapse: collapse;
       margin: 8%;
       min-width: 400px;
       border-radius: 5px 5px 0 0;
       overflow: hidden;
       box-shadow: 0 0 20px rgba(0,0,0,0.1);

    thead tr{
       background-color: $highlight;
       color: $backgroundSecond;
       text-align: left;
       font-weight: bold;
   }
    
    th, td{
        padding: 12px 15px;
        text-align: left;
    }
    
    tbody tr{
        border-bottom: 1px solid #ddd;
    }

    tbody tr:nth-child(even){
        background-color: $backgroundSecond;
    }

    tbody tr:last-of-type{
        border-bottom: 2px solid $extra;
    }
   }

   
</style>