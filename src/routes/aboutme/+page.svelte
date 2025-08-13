<script>
    import pfp from "$lib/assets/ChatGPT Image May 2, 2025, 08_16_57 PM.png"
    import frankcover from "$lib/assets/artworks-6nxYqVnR1zgGoZa1-LzVTvw-t500x500.jpg"
    import videoimage from "$lib/assets/adams_hand.jpg"
    import picture from "$lib/assets/human Anatomy.png"
    import Nav from "$lib/components/Nav.svelte";
</script>
<div class="flex flex-col min-h-screen py-6 text-left w-screen bg-white h-auto items-center ">
    <Nav/>
    <!-- headline -->
    <div class="mt-40 flex w-160 justify-between ">
        <div class="flex flex-col">
            <h1 class="font-bold text-4xl">About Me</h1>
            <div class="max-w-80 mt-4">
                <p class="text-xl text-wrap ">B.Sc. Computer Science student at <span class="text-blue-500">Kathmandu University</span>, Nepal.</p>
                <p class="text-xl text-wrap "> Enjoys <span class="text-green-500">music,</span> <span class="text-purple-500">cinematography</span> & <span class="text-pink-500">drawing.</span></p>
            </div>
        </div>
        <div class="w-56 h-62 p-2 rotate-12 shadow-lg bg-blue-700">
            <div class="w-full h-48 overflow-hidden bg-slate-200">
                <img src={pfp} alt="">
            </div>
        </div>
    </div>
    <!-- music player -->
    <div class="w-160">
        <div class="w-46 h-64 rotate-346 rounded-3xl bg-green-500  ">
             <div class="mt-40 h-60 w-44  rounded-3xl p-2 bg-zinc-100">   
                 <!-- music-player-in -->
                 <div class=" w-full h-full rounded-3xl p-1 button-back">   
                     <div class="h-full w-full rounded-3xl flex justify-between flex-col p-2 button-front">
                         <!-- top-player -->
                         <div class=" w-full h-[60%] rounded-3xl p-1 button-back">   
                             <div class="h-full w-full rounded-3xl button-front overflow-hidden object-fill">
                                <img src="{frankcover}" alt="">
                             </div>
                         </div>
                         <!-- bottom-player -->
                         <div class=" w-full  mt-2 flex h-16 rounded-2xl p-1 button-back  ">   
                             <div class="h-full w-full flex gap-2 p-2 rounded-2xl button2-front">
                                 <!-- play-pause-button -->
                                 <div class=" w-10 h-10 rounded-full p-[1px] button-back ">   
                                     <div class="h-full w-full flex items-center justify-center rounded-full bg-zinc-700">
                                         <!-- pause logo -->
                                          <p>👻</p>
                                     </div>
                                 </div>
                                 <!-- song name -->
                                  <div class="flex flex-col items-center justify-content">
                                      <span class="text-[10px] text-zinc-700">Frank Ocean</span>
                                      <span class="">Trouble</span>
                                  </div>
                                 </div>
                         </div>
                         
                     </div>
                 </div>
             </div>  
         </div>
    </div>
    <!-- video player -->
    <div class="w-160 flex justify-end">
        <div class="h-90 mt-30 w-124 rounded-3xl rotate-334 bg-purple-500">
            <div class=" h-84 w-120 rounded-3xl p-2 bg-zinc-100">   
                <!-- music-player-in -->
                <div class=" w-full h-full rounded-3xl p-1 button-back">   
                    <div class="h-full w-full rounded-3xl  p-2 button-front">
                        <!-- top-player -->
                        <div class=" w-full h-[74%] rounded-3xl p-1 button-back ">   
                            <div class="h-full w-full rounded-3xl overflow-hidden ">
                                <img src={videoimage} alt="">
                            </div>
                        </div>
                        <!-- bottom-player -->
                        <div class="flex justify-between items-center h-[26%] mx-4">
                             <!-- play-pause-button -->
                             <div class=" w-12  mt-2 flex h-12 rounded-full p-1 button-back  ">   
                                 <div class="h-full w-full flex gap-2 p-2 items-center justify-center rounded-full button2-front">
                                          <p>👻</p>
                                 </div>
                             </div>
                              <div class="flex gap-4">
                                  <div class=" w-12  mt-2 flex h-12 rounded-full p-1 button-back  ">   
                                      <div class="h-full w-full flex gap-2 p-2 rounded-full button2-front">
                                      </div>
                                  </div>
                                  <div class=" w-12  mt-2 flex h-12 rounded-full p-1 button-back  ">   
                                      <div class="h-full w-full flex gap-2 p-2 rounded-full button2-front">
                                      </div>
                                  </div>
                              </div>
                         </div>
                    </div>
                </div>
            </div>  
        </div>
    </div>
    <!-- photo viewer -->
    <div class="w-160 flex ">
        <div class="h-108 mt-60 mb-60 w-104 rounded-3xl rotate-350 bg-pink-500">
            <div class=" h-100 w-100 rounded-3xl p-2 bg-zinc-100">   
                <!-- music-player-in -->
                <div class=" w-full h-full rounded-3xl p-1 button-back">   
                    <div class="h-full w-full rounded-3xl  p-2 button-front">
                        <!-- top-player -->
                        <div class=" w-full h-[74%] rounded-3xl p-1 button-back">   
                            <div class="h-full w-full rounded-3xl button-front overflow-hidden ">
                                <img src={picture} alt="">
                            </div>
                        </div>
                        <!-- bottom-player -->
                        <div class="flex justify-between items-center h-[26%] mx-4">
                             <!-- play-pause-button -->

                              <div class="flex gap-4">
                                  <div class=" w-12  mt-2 flex h-12 rounded-full p-1 button-back  ">   
                                      <div class="h-full w-full flex gap-2 p-2 rounded-full button2-front">
                                      </div>
                                  </div>
                                  <div class=" w-12  mt-2 flex h-12 rounded-full p-1 button-back  ">   
                                      <div class="h-full w-full flex gap-2 p-2 rounded-full button2-front">
                                      </div>
                                  </div>
                              </div>
                         </div>
                    </div>
                </div>
            </div>  
        </div>
    </div>

  </div>