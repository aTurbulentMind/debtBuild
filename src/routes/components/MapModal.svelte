<script>
    import { fade, fly } from 'svelte/transition';
    export let mapurl;
</script>

<!-- the modal-->
<div id="myModal" class="modal" transition:fade>

    <!--modal cont-->
    <div class="modal-content" in:fly={{ y: -500}} out:fade>
        <span class="close" on:click>&times;</span>
        <img src={mapurl} alt="map" />
    </div>

</div>

<style lang="scss">
    @import './src/routes/styles/components';
    /**model backy*/
    .modal{
        display: block; /**hidden by def*/
        position: fixed;/**stay in place*/
        z-index: 1;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        overflow: auto;
        background-color: rgb(0,0,0);
        background-color: rgba(0,0,0,0.4);
    }

    /**modal cont/bx*/

    .modal-content {
        background-color: $backgroundSecond;
        margin: 15% auto;
        text-align: center;
        padding: 20px;
        border: 1px solid #888;
        width: 80%;
    }

    img{
        width: 50%;
    }

    /**close butt*/

    .close{
        color: #aaa;
        float: right;
        font-size: 28px;
        font-weight: bold;
    }

    .close:hover,
    .close:focus{
        color: purple;
        text-decoration: none;
        cursor: pointer;
    }
</style>