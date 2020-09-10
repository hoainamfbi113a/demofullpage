<template>
    <div>
        xin chao day la id
    </div>
</template>

<script>
    export default {
        validate({params}){
            return /^\d+$/.test(params.id)
        }
    }
</script>

<style lang="scss" scoped>

</style>