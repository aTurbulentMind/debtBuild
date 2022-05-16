<script>
    export let heading;
    export let content;

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

   <!-- <div>
        
        <a href={learnmore} target="_blank"><button>Website</button></a>
    </div>-->
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
        width: 80%;
        text-align: left;
        outline: none;
        transition: 0.4s;
        box-shadow: 0 2px 20px 2px $extraExtra;
    }

    button.accordion:hover, button.accordion.active {
        background-color: $backgroundSecond;
    }

    .heading{
        font-size: 1.45vw;
    }

    p{
        text-align: justify;
        padding: 0 10px;
        margin: 3%;
        font-size: 1.35vw;
    }

    /*mods button back color*/
    button.active, button.accordion:hover{
        background-color: $highlight;
    }

    /*style acc panel*/
    .panel{
        padding: 0 18px;
        width: 75%;
        margin:0 6%;
        display: block;
        height: 0;
        overflow: hidden;

        p{
            font-size: 1.35vw;
        }
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

    
    @media (max-width: 768px) {
         button.accordion{
        padding: 15px;
        margin:0 10%;
        width: 80%;
    }

        .heading{
        font-size: 3vw;
    }

        .panel{
        padding: 0 18px;
        width: 70%;
        margin:0 12%;
        overflow: hidden; 

        p{
            font-size: 3.35vw;
            margin: 0 5%;
        }
    }
       
      }

    @media only screen and (min-width: 770px) {}

      	/*Extra Large screens */
    @media only screen and (min-width: 1400px) {}
</style>