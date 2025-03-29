<script lang="ts">
    let number = $state(0)
    function onclick() {
        number = number + 1
    }
</script>

<button {onclick}>Click Me!</button>
<h1>{number}</h1>

<style>
    h1 {
        color: blueviolet;
        padding: 0 1rem;
    }
</style>