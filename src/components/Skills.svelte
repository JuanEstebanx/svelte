<script>
    import { each } from "svelte/internal";

    let skills = [
        {
            id: 1,
            name: "HTML",
        },
        {
            id: 2,
            name: "CSS",
        },
        {
            id: 3,
            name: "JavaScript",
        },
    ];
</script>

<div class="Skills">
    <h3>HABILIDADES</h3>
    <ul>
        {#each skills as { name }, i}
            <li>{name}</li>
        {/each}
    </ul>
</div>

<style>
    .Skills {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    ul {
        margin: 0;
        padding: 0;
        list-style: none;
    }
    li{
        display: inline;
        margin: 0 0 0 0.4em;
    }
</style>
