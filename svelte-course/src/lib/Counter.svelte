<script>
    let count = 0;

    $: string = `You have clicked ${count} times`;

    $: if (count > 5) {
        console.log(`The count is ${count}`);
    }

    const increment = () => {
        count += 1;
    };
</script>

<button on:click={increment}>Clicks {count}</button>
<h3>{string}</h3>
