<script>
    export let segment;
</script>

<style>
    /* Basic reset */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    /* Ensure the body takes full viewport height */
    html, body {
        height: 100%;
        font-family: 'Monaco', monospace;
    }

    /* Flexbox layout to center content */
    .wrapper {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100vh;
        padding: 0 20px;
    }

    /* Header styling */
    header {
        display: flex;
        justify-content: center;
    }

    /* Main content styling */
    main {
        max-width: 960px;
        margin: 29px auto;
    }

    .container {
        max-width: 800px;
        width: 100%;
        background-color: #f9f9f9;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        margin: auto;  /* Ensure it is centered horizontally */
    }

    /* Footer styling */
    footer {
        text-align: center;
    }

    @font-face {
        font-family: 'Monaco';
        src: url('/fonts/Monaco.ttf') format('truetype');
        font-weight: normal;
        font-style: normal;
    }
</style>

<div class="wrapper">
    <header>
        <h1>Welcome to My Web Page</h1>
    </header>
    <main>
        <slot></slot>
    </main>
    <footer>
        <p>© 2024 My Web Page</p>
    </footer>
</div>
