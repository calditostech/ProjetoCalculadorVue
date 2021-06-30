<template>
    <div class="display">
        <button class="button"
             @click="$emit('onCalcButtonClick', label)"
            :class="{ double, triple, operation}">
            {{ label }}
        </button>
    </div>
</template>

<script>
export default {
    props: {
        label: {},
        operation: {type: Boolean},
        double: {type: Boolean},
        triple: {type: Boolean}

    }
}
</script>

<style lang="pt" scoped>

.button {
    font-size: 1.4em;
    background-color: var(--bg-button);
    border: none;
    border-right: var(--border-button);
    border-bottom: var(--border-button);
    outline: none;
}

.button:active {
    background-color: #ccc;
}

.button.double {
    grid-column: span 2;
}

.button-triple {
    grid-column: span 3;
}

.button.operation {
    background-color: #fa8231;
    color: #fff;
}

.button.operation:active {
    background-color: #fa8231cc;
}
</style>