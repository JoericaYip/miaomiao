<template>
    <header id="header">
        <slot></slot>
         <!-- 动态渲染父组件传入的title值 -->
        <h1>{{ title }}</h1>
    </header>
</template>

<script>
export default {
    name : 'Header',
    // 父组件Movie、Cinema、Mine向子组件传值title数据，props声明接受的参数
    props : {
        title : {
            type : String,
            default : '喵喵电影'
        }
    }
}
</script>

<style scoped>
#header{width:100%; height:50px; color: #fff; background: #e54847; border-bottom: 1px solid #e54847; position: relative;}
#header h1{ font-size: 18px; text-align: center; line-height: 50px; font-weight: normal; }
#header i{ position: absolute; left: 5px; top: 50%; margin-top: -13px; font-size: 26px;}
</style>
