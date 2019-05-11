<template>  
    <div>
        <h1>我是son子组件</h1>
    </div>
</template>
<script>
export default {
    data(){
        return{
            msg:"我是子组件的数据"
        }
    },
    mounted(){
        this.$emit("show",this.msg)
    }
}
</script>
<style lang="scss" scoped>
    
</style>