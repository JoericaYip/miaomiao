<template>
    <!-- keep alive 实现缓存，避免多次切换路由每次都渲染一遍页面 -->
    <keep-alive>
        <router-view/>
    </keep-alive>
</template>


