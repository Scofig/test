<script>
    export let bgcolor = "black";
    export let opacity = "1";
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div style="background-color: {bgcolor}; opacity: {opacity}" on:click></div>


<style>
    div {
        width: 100px;
        height: 100px;
    }
</style>