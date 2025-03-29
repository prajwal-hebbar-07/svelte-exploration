<script lang="ts">
    function onclick() {
        console.log("Hello from Prajwal on Button Click!")
    }
    let number1 = 1
</script>

<h1>{number1}</h1>
<p>Hello From Prajwal!</p>
<button {onclick}>Click Me!</button>

<style>
    h1 {
        color: steelblue;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        padding: 1rem;
    }
</style>