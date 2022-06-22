<template>
    <div class="flex bg-black h-8 lg:grid grid-cols-3  h-20 w-full items-center sticky -top-1.5 border-b-2">
        <div class=" text-xl text-white flex p-3">
            <button class="my-4" @click="isOpen=!isOpen"> <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mb-14" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
            </svg></button>

            <a class="mx-3 my-5" href=""><img class="" src="public/images/png/logo_full_bw.png" width="100" height="100"> </a>
            <span class="mx-auto my-4"><input class="rounded-full bg-gray-800 text-gray-300 py-0" type="search" placeholder="trek, albom, artist"></span>

        </div>

        <div class="flex justify-center mb-16">
            <span> <a class="text-xl text-white hover:text-blue-600 " href="">Войти</a> </span>
        </div>

        <div class="flex justify-end mx-3">
            <ul class="flex h-8 w-7  justify-end space-x-3 text-xl mb-16 ">

                <li class="bg-white p-2  rounded-full hover:text-blue-400 "><svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z" />
                </svg></li>
                <li class="bg-white p-2  rounded-full hover:text-blue-400"><svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z" />
                </svg></li>
                <li class="bg-white p-2  rounded-full hover:text-blue-400"><svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z" />
                </svg></li>
            </ul>
        </div>
    </div>

    <section>
        <div class="bg-black">
            <nav :class="isOpen ? 'block' : 'hidden' ">
                <ul class="nav ">
                <span class="flex space-x-1 "><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-12 border-l-2  border-l-blue-500 pl-2" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
               <path stroke-linecap="round" stroke-linejoin="round" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
                </svg> <a href="/blog"> Главная</a>
                </span>

                    <inertia-link :href="route('blog')">
                    <span class="flex gap-2 hover:text-blue-600"><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 012-2h2a2 2 0 012 2m0 10a2 2 0 002 2h2a2 2 0 002-2M9 7a2 2 0 012-2h2a2 2 0 012 2m0 10V7m0 10a2 2 0 002 2h2a2 2 0 002-2V7a2 2 0 00-2-2h-2a2 2 0 00-2 2" />
                   </svg>Блог</span>
                    </inertia-link>

                    <span class="flex space-x-3 hover:text-blue-600"> <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                    <path stroke-linecap="round" stroke-linejoin="round" d="M9 19V6l12-3v13M9 19c0 1.105-1.343 2-3 2s-3-.895-3-2 1.343-2 3-2 3 .895 3 2zm12-3c0 1.105-1.343 2-3 2s-3-.895-3-2 1.343-2 3-2 3 .895 3 2zM9 10l12-3" />
                    </svg> <li> Песни</li></span>

                    <li class="hover:text-blue-600"> Альбомы</li>
                    <li class="hover:text-blue-600">Исполнители</li>
                    <span class="flex space-x-3 hover:text-blue-600"><svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M7 4v16M17 4v16M3 8h4m10 0h4M3 12h18M3 16h4m10 0h4M4 20h16a1 1 0 001-1V5a1 1 0 00-1-1H4a1 1 0 00-1 1v14a1 1 0 001 1z" />
                    </svg><li>Видеo</li></span>

                </ul>
            </nav>

            <div class="p-10  inline-block space-x-10">
                <span><h1 class="text-white font-bold text-4xl px-10 ">Главная</h1></span>
                <div class="md:flex-col space-y-4 lg:space-x-6 mt-14 mix-blend-">
                   <button  class="btn bg-gradient-to-tr from-cyan-400 to-fuchsia-600 ">МУЗЫКАЛЬНЫЙ ТОП</button>
                    <button  class=" bg-gradient-to-r from-purple-500 to-amber-400 text-white uppercase text-lg bg-amber-500  px-14 md:py-0 lg:py-2 rounded-lg hover:scale-105 duration-300 transition-all transform shadow">S.KHALIL PRODUCTION</button>
                </div>

                <div class="py-8 flex justify-between">
                    <span class="text-white uppercase text-xl shadow-white shadow-2xl font-bold">Слушайте</span>
                    <a class="text-white mr-12 hover:text-blue-600" href="">больше музыки </a>
                </div>

                <div class="grid md:grid-cols-1 lg:grid-cols-2 ">
                    <div class="space-y-4  w-11/12 ">

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
                    <div class="space-y-4 w-11/12"  >
                        <audio class="  hover:border-cyan-600 border-2 border-black hover:shadow-inner shadow-2xl w-full " controls>
                            <source src="" type="audio/mp3">
                        </audio>
                        <audio class="  hover:border-cyan-600 border-2 border-black hover:shadow-inner shadow-2xl w-full " controls>
                            <source src="" type="audio/mp3">
                        </audio>
                        <audio class="  hover:border-cyan-600 border-2 border-black hover:shadow-inner shadow-2xl w-full " controls>
                            <source src="" type="audio/mp3">
                        </audio>
                        <audio class=" hover:border-cyan-600 border-2 border-black hover:shadow-inner shadow-2xl w-full " controls>
                            <source src="" type="audio/mp3">
                        </audio>
                    </div>
                </div>

                <div>
                    <div class="py-8 flex justify-between">
                        <span class="text-white uppercase text-xl shadow-white shadow-2xl font-bold">Исследуйте</span>
                        <a class="text-white  hover:text-blue-600" href="">больше альбомов</a>
                    </div>
                    <div class=" gap-2 grid md:grid-cols-1 lg:grid-cols-6 ">
                        <div class="flex flex-col">
                            <video class="w-36 h-48  rounded-md " controls >
                                <source src="" type="video/mp4">
                            </video>
                            <span>
                            <a class="text-lg text-white hover:text-blue-400" href="">Nuriddin Selected Album</a>
                            <h1 class="text-gray-400">Nuriddin</h1>
                        </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-48 rounded-md" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-lg text-white hover:text-blue-400" href="">Nuriddin Selected Album</a>
                            <h1 class="text-gray-400">Nuriddin</h1>
                        </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-48 rounded-md" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-lg text-white hover:text-blue-400" href="">Nuriddin Selected Album</a>
                            <h1 class="text-gray-400">Nuriddin</h1>
                        </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-48 rounded-md" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-lg text-white hover:text-blue-400" href="">Nuriddin Selected Album</a>
                            <h1 class="text-gray-400">Nuriddin</h1>
                        </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-48 rounded-md" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-lg text-white hover:text-blue-400" href="">Nuriddin Selected Album</a>
                            <h1 class="text-gray-400">Nuriddin</h1>
                        </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-48 rounded-md" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-lg text-white hover:text-blue-400" href="">Nuriddin Selected Album</a>
                            <h1 class="text-gray-400">Nuriddin</h1>
                        </span>
                        </div>
                    </div>
                </div>

                <div>
                    <div class="flex justify-between py-8">
                        <span class="text-white uppercase text-xl shadow-white shadow-2xl font-bold">Смотрите</span>
                        <a class="text-white mr-12 hover:text-blue-600" href="">больше клипов</a>
                    </div>
                    <div class=" gap-2 grid md:grid-cols-1 lg:grid-cols-6 ">
                        <div class="flex flex-col">
                            <video class="w-36 h-36" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-sm text-gray-400" href="">Далер Назаров - Чак чаки борон</a>
                            </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-36" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-sm text-gray-400" href="">Далер Назаров - Чак чаки борон</a>
                            </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-36" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-sm text-gray-400" href="">Далер Назаров - Чак чаки борон</a>
                            </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-36" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-sm text-gray-400" href="">Далер Назаров - Чак чаки борон</a>
                            </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-36" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-sm text-gray-400" href="">Далер Назаров - Чак чаки борон</a>
                            </span>
                        </div>

                        <div class="flex flex-col">
                            <video class="w-36 h-36" controls >
                                <source src="" type="vide/mp4">
                            </video>
                            <span>
                            <a class="text-sm text-gray-400" href="">Далер Назаров - Чак чаки борон</a>
                            </span>
                        </div>
                    </div>
                </div>

                <div>
                    <div class="py-8 flex justify-between">
                        <span class="text-white uppercase text-xl shadow-white shadow-2xl font-bold">Читайте</span>
                        <a class="text-white mr-12 hover:text-blue-600" href="">больше статей</a>
                    </div>
                </div>

                <div class="my-8 space-x-6 grid lg:grid-cols-4 ">

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
        </div>
        <audio class="sticky -bottom-1.5 w-full" controls>
            <source src="horse.ogg" type="audio/ogg">
            <source src="horse.mp3" type="audio/mpeg">
        </audio>
    </section>

<Blog>

</Blog>

 <Contastants>

 </Contastants>
    <div id="nav">
        <router-link to="/blog">Blog</router-link>
        <router-view/>
    </div>




</template>

<script>
import Blog from  "./Blog";
import Contastants from "./Contastants";
export default {
    components: {Contastants, Blog},
    data(){
        return{
           isOpen:false,
        }
    },
}
</script>
<style>

</style>
