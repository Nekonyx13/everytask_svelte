<script>
    import { CheckCircle, Sheet, Users, Settings } from "lucide-svelte";
</script>

<nav class="nav-bar">
    <div class="nav-item">
        <CheckCircle size="35" strokeWidth="2" />
    </div>
    <div class="nav-item">
        <Sheet size="35" strokeWidth="2" />
    </div>
    <div class="nav-item">
        <Users size="35" strokeWidth="2" />
    </div>
    <div class="nav-item">
        <Settings size="35" strokeWidth="2" />
    </div>
</nav>

<style lang="scss">
    .nav-bar {
        position: fixed;
        bottom: 0;
        width: 100%;
        height: 5rem;

        display: flex;
        justify-content: space-around;
        align-items: center;
        border-top-left-radius: 1em;
        border-top-right-radius: 1em;
        background-color: #f5fbfe;
        box-shadow: 0px -28px 27px 20px #f5fbfe;
        padding-bottom: 1em;
        padding-top: 1em;

        .nav-item {
            color: #5c2372;
            font-size: 0px;
            background: #f5fbfe;
            border-radius: 1rem;
        
            padding: 20px;

            transition: all 0.5s;

        }
    }

    
    .nav-item:hover {
                box-shadow: 5px 5px 10px #d0d5d8, -5px -5px 10px #ffffff;
            }
    @media (min-width: 640px) {
        .nav-bar {
            width: 640px;
        }
    }
</style>
