<script lang="js">
  let { page = '' } = $props();
</script>

<main class="topbar">
    <div class="buttons">
        <a href="/" class:active={page === 'home'}>Home</a>
        <a href="/wiki" class:active={page === 'wiki'}>Wiki</a>
    </div>

    <div class="promo">
        <p>Solar Engine</p>
    </div>
</main>

<style>
    .topbar {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem;
        background-color: rgba(0, 0, 0, 0.25);
        backdrop-filter: blur(4px);
        
        .promo {
            p:hover {
                animation: spin 1s linear infinite;
            }
        }
        
        .buttons {
            display: flex;
            gap: 0.5rem;
            
            a {
                color: white;
                text-decoration: none;
                background-color: rgba(0, 0, 0, 0.5);
                padding: 0.75rem 1.5rem;
                border-radius: 0.5rem;
                scale: 1;
                transition: scale 0.2s;
            } a:hover {
                scale: 1.1;
            } a.active {
                animation: spin 500ms ease both;
            }
        }
    }

    @keyframes spin {
        from{
            transform: rotate(0deg);
        }
        to{
            transform: rotate(360deg);
        }
    }
</style>