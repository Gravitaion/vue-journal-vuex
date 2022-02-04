<template>
    <button class="btn btn-primary">
        <i :class="classIcon"></i>
    </button>
</template>

<script>
export default {
    props: {
        icon: {
            type: String,
            default: 'fa-plus'
        }
    },
    computed: {
        classIcon() {
            return `fa fa-2x ${ this.icon }`
        }
    }
}
</script>

<style lang="scss" scoped>
    button {
        border-radius: 100%;
        bottom: 20px;
        height: 80px;
        position: fixed;
        right: 20px;
        width: 80px;
    }
</style>