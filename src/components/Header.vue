<template>
    <div id="header">
        <div class="flex w-full bg-black max-h-32 text-white border-b p-8">
            <div class="flex flex-col w-full hidden md:flex items-end justify-center pr-4">
                <h2 class="text-2xl">{{ titulo }}</h2>
                <a class="text-xl"><strong></strong>{{ entrega }}</a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            titulo: 'Angel Nicolas Jimenez',
            entrega: 'VueJs 3'
        }
    },
}
</script>

<style>

</style>