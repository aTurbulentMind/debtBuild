<script>
    export let heading;
    export let content;
    export let learnmore;

    let isOpen = false;
</script>

<button class:active={isOpen} class="accordion" on:click={() => isOpen = !isOpen}>
    <span class="heading">{heading}</span>
    {#if isOpen}
    <span class="icon">&minus;</span>
    {:else}
    <span class="icon">&plus;</span>
    {/if}
</button>

<section class="panel" class:open-panel={isOpen}>
    <p>{content}</p>

    <div>
        <button on:click>Logo</button>
        <a href={learnmore} target="_blank"><button>Website</button></a>
    </div>
</section>

<style lang="scss">

    @import 'styles/components';

    
 /*style open button*/
    
    button.accordion{
        background-color: $backgroundHallow;
        cursor: pointer;
        padding: 15px;
        margin:0 5%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        border: .5px solid $extra;
        width: 80%;
        text-align: left;
        outline: none;
        transition: 0.4s;
        
    }

    button.accordion:hover, button.accordion.active {
        background-color: $backgroundSecond;
    }

    .heading{
        font-size: 1.5rem;
    }

    p{
        font-size: 1.2rem;
        text-align: justify;
        padding: 10px 10px 5px;
        margin: auto 0;
    }

    /*mods button back color*/
    button.active, button.accordion:hover{
        background-color: $highlight;
    }

    

    /*style acc panel*/
    .panel{
        padding: 0 18px;
        width: 70%;
        margin:0 6%;
        display: block;
        height: 0;
        overflow: hidden;
    }

    .open-panel{
        height: 170px;
    }

    span.icon {
        font-size: 1.8rem;
    }

    section.panel{
        display: flex;
        flex-direction: column;
        align-items: center;
        height: 0;
        overflow: auto;
        transition: all .5s;
    }

    section.open-panel{
        height: 170px;
        box-shadow: inset 0 0 5px black;
    }

    section.open-panel div{
        width: 100%;
        display: flex;
        justify-content: center;
    }

    section div button {
        width: 150px;
        font-weight: bold;
        padding: 10px 0;
        margin: 10px 10px 20px;
        cursor: pointer;
    }

    div button:active {
        background-color: hsl(213, 63%, 34%);
    }
 
</style>