<script>
    export let type, onClick, children;
</script>

<button type={type} onClick={onClick}>
    { children }
</button>

<style>
    button {
        margin: 0 auto;
        padding: 0.5rem 1rem;
        border: 1px solid black;
        color: inherit;
        text-decoration: none;
        background-color: transparent;
        box-shadow: 2px 2px 0 black;
        cursor: pointer;
    }
</style>
