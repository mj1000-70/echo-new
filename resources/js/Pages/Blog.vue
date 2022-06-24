<template>
    <div class="px-20 bg-black">
        <div class="">
            <div class="space-y-2">
                <span class="text-white text-4xl shadow-white font-bold">Блог</span>
            </div>
        </div>

        <div class="py-8 space-x-6 grid lg:grid-cols-4 inline-block">

            <div class="flex flex-col hover:scale-105 duration-300 transition-all transform ">
                <img class=" border-2" src="public/images/png/logo_full_bw.png" width="200" height="250">
                <span class="text-white text-2xl mt-2">Сборники и альбомы</span>
                <p class="text-gray-400 space-y-4 text-md">
                    Далер Назаров рассказывает об
                    истории своих первых неофициальных
                    альбомов, о важности соблюдения
                    хронологического порядкаи
                    разниe между тематическим
                    альбомом и сборником.
                    <span class="text-sm"> 09.06.2020 Далер Назаров</span> </p>


            </div>

            <div class="flex flex-col hover:scale-105 duration-300 transition-all transform ">
                <img class=" border-2" src="public/images/png/logo_full_bw.png" width="200" height="250">
                <span class="text-white text-2xl mt-2"> О записи</span>
                <p class="text-gray-400 w-72 text-md">

                    Сегодня для нас ценно схваченное мгновение,
                    в котором ещё не остыло состояние, принесённое
                    вдохновением новой песни. Её надо моментально
                    фиксировать, это и будет её единственный след.
                    <span class="text-sm"> 13.07.2020 Далер Назаров 0:00</span> </p>
            </div>
        </div>
    </div>



</template>

<script>
export default {
    name: "Blog"
}
</script>

<style scoped>

</style>
