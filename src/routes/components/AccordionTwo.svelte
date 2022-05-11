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

    @import './src/routes/styles/components';

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
        width: 85%;
        text-align: left;
        outline: none;
        transition: 0.4s;
        
    }

    button.accordion:hover, button.accordion.active {
        background-color: $backgroundSecond;
    }

    p{
        text-align: justify;
        padding: 0 10px;
        margin: 3%;
    }

    /*mods button back color*/
    button.active, button.accordion:hover{
        background-color: $highlight;
    }

    /*style acc panel*/
    .panel{
        padding: 0 18px;
        width: 75%;
        margin:0 8%;
        display: block;
        height: 0;
        overflow: hidden;
    }

    .open-panel{
        height: 210px;
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
        transition: all .25s;
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
        padding: 7px 0;
        margin: 10px 10px 20px;
        cursor: pointer;
    }

    div button:active {
        background-color: hsl(213, 63%, 34%);
    }
</style>