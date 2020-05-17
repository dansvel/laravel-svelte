<script>
    import { onMount } from "svelte";
    onMount(() => {
        console.log("the component has mounted");
    });

    let links = [
        { text: 'Laravel', url: 'https://laravel.com/'},
        { text: 'Inertia', url: 'https://inertiajs.com/'},
        { text: 'Svelte', url: 'https://svelte.dev/'}
    ];
</script>

<style>
    .full-height {
        height: 100vh;
    }

    .flex-center {
        align-items: center;
        display: flex;
        justify-content: center;
    }

    .position-ref {
        position: relative;
    }

    .content {
        text-align: center;
    }

    .title {
        font-size: 84px;
    }

    .links > a {
        color: #636b6f;
        padding: 0 25px;
        font-size: 13px;
        font-weight: 600;
        letter-spacing: .1rem;
        text-decoration: none;
        text-transform: uppercase;
    }

    .m-b-md {
        margin-bottom: 30px;
    }
</style>

<svelte:head>
    <title>Laravel and Svelte with Inertia</title>
    <link href="https://fonts.googleapis.com/css?family=Nunito:200,600" rel="stylesheet">
    <style>
        html, body {
            background-color: #fff;
            color: #636b6f;
            font-family: 'Nunito', sans-serif;
            font-weight: 200;
            height: 100vh;
            margin: 0;
        }
    </style>
</svelte:head>

<div class="flex-center position-ref full-height">
    <div class="content">
        <div class="title m-b-md">
            Hello World
        </div>

        <div class="links">
            {#each links as link}
                <a href="{link.url}">{link.text}</a>
            {/each}
        </div>
    </div>
</div>
