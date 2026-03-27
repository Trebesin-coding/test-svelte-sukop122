<script>
    import { shared } from "$lib/shared.svelte";

    function pointer() {
        if (shared.emoji === "🙂"){
            shared.score += 1
        } else {
            shared.score -= 1
        }
    }
</script>

<button onclick={pointer}>+</button>

<style>
    button {
        background-color: aqua;
        border-radius: 10000px;
    }
</style>