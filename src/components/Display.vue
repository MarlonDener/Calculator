<template>
    <div class="display">
        {{value}}
    </div>
</template>

<script>
    export default{
        props: ['value']   
    }
</script>

<style>
.display{
    grid-column: span 4;
    background-color: rgba(204, 204, 204, 0.267);
    display: flex;
    justify-content: flex-end;
    padding: 30px 15px;
    font-size: 1.8em;
}

</style>