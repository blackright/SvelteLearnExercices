<script>
    //export let title = "This is My Button Prop";
    export let size = 'small';
    export let shadow = false;
</script>

<button 
    class={size == 'large' ? 'size-lg' : 'size:sm'}
    class:shadow><slot />
</button>

<style lang="scss">
    button {
        border-radius: 10px;
        border-color: brown;
        color:blanchedalmond;
        cursor: pointer;
        &:hover {
            background-color: black;
            background-image: linear-gradient(rgba(0,0,0,0.4) 0 0);
        }
        &:active {
            background-image: linear-gradient(rgba(255,255,255,0.1) 0 0);
        }
        &.size-sm {
            padding: 20px 25px 20px 25px;
        }
        &.size-lg {
            padding: 25px 30px 25px 30px;
            font-size: 25px;
        }
        &.shadow {
            box-shadow: 0 0 20px;
        }
    }
</style>