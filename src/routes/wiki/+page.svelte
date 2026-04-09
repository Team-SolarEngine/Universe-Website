<script lang="js">
    import Topbar from '../../webpack/topbar.svelte';
    const page = 'wiki';
</script>

<main>
    <Topbar page={page}/>
    
    <span>maybe later...</span>
</main>

<style>
    span {
        left: 50%;
        top: 50%;
        position: absolute;
        transform: translate(-50%, -50%);
    }
</style>