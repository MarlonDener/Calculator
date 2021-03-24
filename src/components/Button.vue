<template>
    <button class="button" @click="$emit('onCalcButtonClick',label)" :class="{double, triple, operation}">
        {{label}}
    </button>
</template>

<script>
    export default{
        props:{
            label: {},
            operation: {type:Boolean},
            double: {type:Boolean},
            triple: {type:Boolean}
        }
    }

</script>

<style>
    :root{
        --bg-button: #f0f0f0;
        --border-button: solid 1px #888;
    }
    button{
        padding: 18px;
        background-color: var(--bg-button);
        border: none;
        border-right: var(--border-button);
        border-bottom: var(--border-button);
        outline: none;
        cursor: pointer;
    }
    button:hover{
        background-color: rgb(211, 211, 211);
    }
    button:active{
        background: rgb(94, 94, 94);
        color:#fff;
    }
    button.double{
        grid-column: span 2;
    }
      button.triple{
        grid-column: span 3;
    }
    button.operation{
        background-color: #fa8231;
        color: #fff;
    }
    button.operation:active{
        background-color: #fa8231cc;
    }
</style>