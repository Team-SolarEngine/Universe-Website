<script lang="js">
    import Topbar from '../../webpack/topbar.svelte';
    const page = 'wiki';
</script>

<main>
    <Topbar page={page}/>

    <span>
        <div class="main">
            <div class="mainContent background">
                <section class="info">
                    The Wiki is not currently ready, take some commonly known bugs instead!<br>
                    <br>
                    <br>
                    <b>Compiling Issues: </b><br>
                    Unknown class MP4Handler |  Downgrade hxCodec to 2.5.1 <code>haxelib set hxCodec 2.5.1</code><br>
                    <br>
                    discord_rpc | "fatal error C1083: Cannot open include file: '../lib/discord-rpc/include/discord-rpc.h': No such file or directory" | do NOT directly install discord_rpc, run <code>haxelib git discord_rpc https://github.com/Aidan63/linc_discord-rpc</code> <br>
                    <br>
                    <br>
                    <b>Game Issues: </b><br>
                    <b> Windows: </b><br>
                    Certain lua based HUD elements are not colored correctly/at all - This will be fixed in a minor patch, if you downloaded 0.6.0's windows build, update to 0.6.1 when it releases.<br>
                    <br>
                    <b> Universal: </b><br>
                    Result Screen does not properly exit song in some cases - Fixed in 0.6.1
                </section>
            <div>
        </div>
    </span>
</main>

<style>
    span {
        left: 50%;
        top: 50%;
        position: absolute;
        transform: translate(-50%, -50%);
    }
</style>
