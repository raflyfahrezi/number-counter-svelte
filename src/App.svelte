<script>
    //import
    import Button from './components/Button.svelte'

    // initialize variables
    let name = ''

    // functions
    const plusNumberHandler = () => {}

    const minusNumberHandler = () => {}

    // export variables
    export { name }
</script>

<main>
    <h1>{name}</h1>
    <p>
        Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
        how to build Svelte apps.
    </p>
    <div>
        <Button onClickHandler={plusNumberHandler}>Plus Number</Button>
        <Button onClickHandler={minusNumberHandler}>Minus Number</Button>
    </div>
</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    h1 {
        color: #ff3e00;
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
