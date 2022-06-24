<template>
    <div class="bg-black px-20">
        <div class="flex flex-col space-y-2">
            <span class="text-white uppercase text-4xl shadow-white font-bold">Песни</span>
            <a class="text-white mr-12 hover:text-blue-600" href="">виыбрат жанр</a>
        </div>

            <div class=" py-8  w-full grid gap-y-4 inline-block">
                <audio class="  hover:border-cyan-600 border-2 border-black w-full hover:shadow-xl" controls>
                    <source src="" type="audio/mpeg">
                </audio>

                <audio class="  hover:border-cyan-600 border-2 border-black w-full hover:shadow-inner shadow-2xl " controls>
                    <source src="" type="audio/mp3">
                </audio>
                <audio class="  hover:border-cyan-600 border-2 border-black w-full  hover:shadow-inner shadow-2xl" controls>
                    <source src="" type="audio/mp3">
                </audio>
                <audio class="  hover:border-cyan-600 border-2 border-black w-full  hover:shadow-inner shadow-2xl" controls>
                    <source src="" type="audio/mp3">
                </audio>
            </div>

    </div>

</template>

<script>
export default {
    name: "Songs"
}
</script>

<style scoped>

</style>
