<template>
    <div class="dialog">
        <div class="dialog__content">
            <slot></slot>
        </div>
    </div>
</template>

<script>
export default {
    name: "my-dialog",
    props: {
        show: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style scoped>
.dialog {
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    background: rgba(0, 0, 0, 0.5);
    position: fixed;
    display: flex;
}
.dialog__content {
    margin: auto;
    margin-top: 0;
    background: #fff;
    border-radius: 0 0 16px 16px;
    width: 90%;
    min-height: 100px;
    padding: 40px;
    text-align: center;
}
</style>