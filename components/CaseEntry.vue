<template>
        <div class="casevideo relative aspect-w-16 aspect-h-9 pb-16">
            <div class="project-title w-full text-5xl absolute top-1/2 transform -translate-y-1/2 "> {{projectInfo.title}} </div>
            <video class="object-cover rounded-lg" src="~assets/videos/dummy-video.mp4" autoplay loop muted ></video>
        </div>
</template>

<script>
    export default {
        props: [
            "projectInfo"
        ]
    }
</script>

<style scoped>

</style>