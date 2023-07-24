<script>
    export let initialCount;
    export let maxCount;

    let count = initialCount;

    const increment = () => {
        if (count === maxCount) return;
        count += 1;
    };
</script>

<button on:click={increment}>Clicks {count}</button>
