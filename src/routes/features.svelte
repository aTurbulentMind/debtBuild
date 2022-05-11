<script>
    import { Packs } from './feats/Packs.js';//This is the info for each table
    
    import Accordion from './components/Accordion.svelte'; //the structure of the accordian
    
    let continentMap = "";

</script>


<header>
    <h1>Features or Packages</h1>
    
    <p>Debt$Net® features Lorem ipsum dolor sit, amet consectetur adipisicing elit. Doloribus itaque enim omnis assumenda, quis ducimus, ut voluptatem recusandae expedita eligendi veniam, non pariatur nesciunt dolore optio quidem fugit architecto! Quod adipisci voluptatum maxime, nam, numquam repellat officia quos nostrum deleniti distinctio, sunt laudantium porro debitis itaque! Corrupti, molestias facere reprehenderit autem quia, nesciunt laborum possimus vitae itaque culpa perferendis odit perspiciatis esse voluptatibus? Consequuntur tempore quod voluptatibus hic quidem, esse corrupti laboriosam deleniti fuga illum aut ratione est id exercitationem reprehenderit!</p>
</header>

<!--this is where the accordion starts-->

<h2>Packages:</h2>



{#each Packs as {heading, content, learnurl}}
<Accordion {heading} 
           {content}
           learnmore={learnurl}
            />
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