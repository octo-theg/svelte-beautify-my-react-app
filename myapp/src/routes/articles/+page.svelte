<script>
    import {onMount} from "svelte";
    import Header from "../../components/Header/Header.svelte";
    import Footer from "../../components/Footer/Footer.svelte";
    import Nested from '../../components/Nested.svelte';

    let articles = []
    onMount(async () => {
        const articlesResponse = await fetch('https://jsonplaceholder.typicode.com/posts')
        articles = await articlesResponse.json()
    })

    let count = 1;
    $: doubled = count * 2;

    function handleClick() {
        count += 1;
    }

</script>

<Header/>
    <main>
    <h1>Yes les articles</h1>

    {#each articles as article}
        {#if article.title.charAt(0) === 't'}
            <h3>{article.title}</h3>
            <p>{article.body}</p>
        {/if}
    {/each}
    <button on:click={handleClick}>Clique moi pour doubler {count}</button>
    {doubled}

    <Nested answer={42}/>
</main>
<Footer/>


