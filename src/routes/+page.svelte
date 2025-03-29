<script lang="ts">
    let number = $state(0)
    let udpateHintText = $derived(number === 0 ? "Hey! Why don't you click on the button" : `You have clicked ${number} times!`)

    function onclick() {
        number = number + 1
    }
</script>

<button {onclick}>Click Me!</button>
<h1>{number}</h1>

<!-- This below line is one of the ways of updating conditional data -->
<!-- <p>{number === 0 ? "Hey! Why don't you click on the Button?" : `You have clicked ${number} times!`}</p> -->
 <p>{udpateHintText}</p>

<style>
    h1 {
        color: blueviolet;
        padding: 0 1rem;
    }
</style>