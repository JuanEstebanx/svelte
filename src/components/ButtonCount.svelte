<script>
    import {count} from "../store/store.js";
    function handlCick(){
        count.update( n => n + 1);
    }

</script>

<style>
    button{
        background-color: orange;
        border:none;
        color:white;
        border-radius: 4px;
        padding: 0.5rem;
        text-transform: uppercase;
        cursor: pointer;
    }
</style>


<button on:click={handlCick}>
    Click {$count == 0 ? '' : $count }
</button>