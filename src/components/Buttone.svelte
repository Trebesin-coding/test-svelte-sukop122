<script>
import { shared } from "$lib/shared.svelte";
let clickd = false

function change() {
    if (shared.emoji === "🙂") {
        clickd = true
        shared.emoji = "😢"
    } else {
        shared.emoji = "🙂"
        clickd = false
    }
}

if (clickd === true) {

}
</script>
<button onclick={change}>{shared.emoji}</button>
<style>
    button {
        background-color: rgb(255, 0, 0);
        border-radius: 10000px;
    }
</style>