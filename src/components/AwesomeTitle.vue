<template>
    <div style="padding-bottom: 30px">
        <h1 class="heading-bg bg-vue font-montserrat" :style="{'background-color': bgColor, 'color': textColor}">{{title}}</h1>
    </div>
</template>
<script>
export default {
    name: 'AwesomeTitle',
    props: ['title', 'bgColor', 'textColor'],
}
</script>
<style lang="scss" scoped>
.heading-bg {
    padding-left: 30px;
    padding-right: 30px;
    clip-path: polygon(10% 0, 100% 0%, 90% 100%, 0% 100%);
    text-align: center;
    text-transform: uppercase;
    font-weight: 500;
}
</style>


