<template> 
	<div>
		<h1>我是App父组件----{{mydata}}</h1>
		<son @show="show"></son>
	</div>
</template>
<script>
import son from "./son.vue"
export default {
	data(){
		return{
			mydata:""
		}
	},
	methods:{
		show(data){
			this.mydata=data
		}
	},
	components:{
		son
	}
}
</script>
<style lang="scss" scoped>
  
</style>