<template>
    <div class="search">
        <input type="search" placeholder="Type in a beer">
        <button>🔎</button>
    </div>
</template>

<script>
export default {
    name: 'search'    
}
</script>

<style lang="less" scoped>
    .search {
        display: flex;
        max-width: 32rem;
        margin: 0 auto;

        @border-color: #a1020c;
        @border-radius: 1rem;

        input {
            flex: 1;
            padding: 0.5rem 1rem;
            border: 1px solid @border-color;
            border-right: none;
            border-top-left-radius: @border-radius;
            border-bottom-left-radius: @border-radius;
            outline: none;
            color: @border-color;

            &::placeholder {
                color: lighten(@border-color, 30%);
            }
        }

        button {
            background: transparent;
            border: 1px solid @border-color;
            border-left: none;
            border-top-right-radius: @border-radius;
            border-bottom-right-radius: @border-radius;
            outline: none;
        }
    }
</style>