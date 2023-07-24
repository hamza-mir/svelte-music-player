<script>
    let count1 = 0;
    let count2 = 0;

    const setCount2 = (x) => {
        count2 = x;
    };

    $: setCount2(count1);
    $: string = `Count2 is ${count2}`;

    const increment1 = () => {
        count1 += 1;
    };
</script>

<button on:click={increment1}>Clicks {count1}</button>
<p>{string}</p>
