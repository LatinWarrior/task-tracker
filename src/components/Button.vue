<template>
    <button @:click="onClick" :style="{ background: color }" class="btn">
        {{ text }}
    </button>
</template>

<script lang="js">
export default {
    // eslint-disable-next-line
    name: 'Button',
    props: {
        text: String,
        color: String
    },
    methods: {
        onClick() {
            console.log(`click`);
            this.$emit('btn-click')
        }
    }
};
</script>
