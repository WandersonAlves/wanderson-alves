<template>
    <div class="container">
        <div class="container-padding">
            <div class="flex flex-column flex-align-center" style="margin: 40px 0;">
                <awesome-title title="skills" bgColor="#e64980" textColor="#e3c0c0"></awesome-title>
            </div>
            <div class="flex flex-row flex-wrap flex-justify-center responsive-column">
                <circle-progress v-for="skill of skills" class="item" direction="mid" color="#514444" :percentage="skill.value" :skill="skill.name" :description="skill.description"></circle-progress>
            </div>
        </div>
    </div>
</template>
<script>
import AwesomeTitle from '@/components/AwesomeTitle.vue';
import CircleProgress from '@/components/CircleProgress.vue';

export default {
    name: 'Skills',
    components: {
        AwesomeTitle,
        CircleProgress
    },
    data() {
        return {
            skills: [
                {
                    name: 'JavaScript',
                    value: 95,
                    description: 'Closures, functional programming, Object.assign({}, obj);'
                },
                {
                    name: 'VueJS',
                    value: 80,
                    description: 'Vuex, vue-router, mixins'
                },
                {
                    name: 'Angular 4+',
                    value: 80,
                    description: 'TypeScript, routeGuards, rxjs'
                },
                {
                    name: 'Git',
                    value: 75,
                    description: 'Rebase, cherry-pick, merges'
                },
                {
                    name: 'HTML 5',
                    value: 75,
                    description: 'Personal sites and corporate systems. Web apps'
                },
                {
                    name: 'CSS/SCSS',
                    value: 63,
                    description: 'Media queries, BEM, box-shadow, ::before'
                },
                {
                    name: 'Photoshop',
                    value: 55,
                    description: 'Prototypes, image manipulation'
                },
                {
                    name: 'Sketch App',
                    value: 50,
                    description: 'Prototypes'
                },
                {
                    name: 'Jenkins',
                    value: 38,
                    description: 'Pipelines, Groovy Files'
                },
                {
                    name: 'NodeJS',
                    value: 38,
                    description: 'It\'s JavaScript anyway'
                },
                {
                    name: 'React',
                    value: 25,
                    description: 'Learning'
                },
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
.container {
  min-height: 100vh;
  width: 100vw;
  padding: 65px 0;
  background-color: #e3c0c0;
}
.item {
    max-width: 20%;
    width: 20%;

    @media (max-width: 768px) {
        max-width: 100%;
        width: 100%;
    }
}
.container-padding {
    @media (max-width: 768px) {
        padding: 0 25px;
    }
}
.responsive-column {
    @media (max-width: 768px) {
        flex-direction: column;
        align-items: center;
    }
}
</style>


