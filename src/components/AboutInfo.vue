<template>
    <div class="flex flex-column">
        <h3 class="font-montserrat">{{title}}</h3>
        <p>{{value}}</p>
    </div>
</template>
<script>
export default {
    name: 'AboutInfo',
    props: ['title', 'value']
}
</script>
<style lang="scss" scoped>
h3 {
    font-weight: 500;
    font-size: 24px;
    color: #e64980;
    text-transform: uppercase;
}
p {
    font-size: 1em;
    font-weight: 300;
}
div {
    @media (max-width: 768px) {
        text-align: center;
    }
}
</style>


