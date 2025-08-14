<script>
    import pfp from "$lib/assets/ChatGPT Image May 2, 2025, 08_16_57 PM.png"
    import frankcover from "$lib/assets/artworks-6nxYqVnR1zgGoZa1-LzVTvw-t500x500.jpg"
    import videoimage from "$lib/assets/adams_hand.jpg"
    import playIcon from "$lib/assets/play-1000-svgrepo-com.svg"
    import Nav from "$lib/components/Nav.svelte";
    import FregSong from "$lib/assets/A$AP Ferg - Dreams, Fairytales, Fantasies (Official Audio) ft. Brent Faiyaz, Salaam Remi.mp3"
    import FrankSong from "$lib/assets/Trouble - Frank ocean (Lyrics).mp3"
    import JoelSong from "$lib/assets/Billy Joel - Vienna (Official Video).mp3"
    
    import { gsap } from "gsap";
    import { TextPlugin } from "gsap/TextPlugin";
    import { SplitText } from "gsap/SplitText";
    import { onMount } from "svelte";

gsap.registerPlugin(TextPlugin);
onMount(()=>{
  let split;
  SplitText.create("#head-1",{
    type:"words,lines",
    linesClass:"line",
    mask:"lines",
  onSplit:(self)=>{
    split=gsap.from(self.lines,{
      duration:0.8,
      yPercent:100,
      opacity :0,
      stagger:0.1,
      ease: "expo.out",

      onComplete:()=>{
        split.revert()
      }
    })
    return split;
  }
})
})
    
    function playFreg(song){
        var music = new Audio(song);
        playMusic(music)
    }
    function playJoel(song){
        var music = new Audio(song);
        playMusic(music)
    }
    function playFrank(song){
        var music = new Audio(song);
        // music.play()
        playMusic(music)
    }

    function playMusic(music){
        music.play();
    }
    // make stop button


</script>
<div class="flex flex-col min-h-screen py-6 text-left w-screen bg-white h-444 items-center ">
    <Nav/>
    <!-- headline -->
    <div class="mt-40 flex flex-row w-160 justify-between items-start">
        <div id="head-1" class="flex p-4 flex-col">
            <p class="text-4xl">About <span class="font-bold">Me</span> </p>
            <div class="max-w-80 mt-4">
                <p class="text-xl text-wrap ">B.Sc. Computer Science student at <span class="text-blue-500">Kathmandu University</span>, Nepal.</p>
                <p class="text-xl text-wrap "> Enjoys <span class="text-green-500">music,</span> <span class="text-purple-500">cinematography</span> & <span class="text-pink-500">drawing.</span></p>
            </div>
        </div>
        <div id="head-1" class=" justify-end flex rotate-6">
                <div class="justify-end w-full  flex rotate-12 ">
                    <button class="relative hover:cursor-crosshair bg-pink-500 h-8 w-4">
                        ;)
                    </button>
                </div>
                <div class="w-50 h-50 overflow-hidden p-2 shadow-lg bg-blue-700  border-blue-700">
                    <img src={pfp} alt="" width="192px" class="flex">
                </div>
        </div>
    </div>
    <!-- music player --> 
    <div class="w-160 mt-30">
        <div class=" rotate-346 relative w-42 h-66 p-1 button-back hover:gap-2  border-b-14  border-green-500 rounded-4xl hover:p-1 hover:w-90 hover:transition-all duration-400 hover:cursor-pointer">
            <div class="w-full h-full hover:gap-2 group flex rounded-3xl bg-zinc-700   hover:transition-all duration-400 hover:cursor-pointer">
               <!-- music-player-in -->
                <div class="min-w-40 max-w-40  flex min-h-full max-h-full rounded-3xl p-1 button-back">   
                    <div class="h-full min-w-full rounded-3xl flex justify-between flex-col p-2 button-front">
                             <!-- top-player -->
                             <div class=" w-full h-[55%] rounded-3xl p-1 button-back">   
                                 <div class="h-full w-full rounded-3xl button-front overflow-hidden  ">
                                    <img src="{frankcover}" alt="">
                                 </div>
                             </div>
                             <!-- bottom-player -->
                             <div class=" w-full  mt-2 flex h-14 rounded-2xl p-1 button-back  ">   
                                 <div class="h-full w-full flex justify-center gap-3 items-center px-[2px]  rounded-2xl button2-front">
                                     <!-- song name -->
                                     <button class="rounded-full hover:shadow-xl hover:bg-zinc-700 flex justify-center items-center bg-zinc-800 hover:cursor-crosshair h-8 w-8" on:click={stopMusic()}>
                                        <img src={playIcon} alt="" height="14px" width="14px" class="hover:opacity-40">
                                     </button>
                                      <div class="flex flex-col items-start px-1 py-1 ">
                                          <p class="text-[9px]  text-zinc-700">FREG</p>
                                          <p class="">Fantasies</p>
                                      </div>
                                     </div>
                             </div>
                    </div>
                </div> 
                  <!-- music-chooser -->
                 <div class=" group-hover:w-full flex group-hover:p-5 group-hover:gap-4 flex-col">
                     <button on:click={playFrank(FrankSong)}  class="w-full hover:cursor-crosshair text-white hidden group-hover:block py-1 px-3 inset-ring hover:bg-green-600 h-14 rounded-xl">
                         <p class="w-full text-nowrap text-sm">Frank Ocean</p>
                         <p class="w-full">Trouble</p>
                     </button>
                    <button on:click={playFreg(FregSong)} class="w-full hover:cursor-crosshair text-white hidden group-hover:block  py-1 px-3 inset-ring hover:bg-green-600 h-14 rounded-xl">
                        <p class="w-full text-nowrap text-sm">FREG</p>
                        <p class="w-full">Fantasies</p>
                    </button>
                    <button on:click={playJoel(JoelSong)} class="w-full hover:cursor-crosshair text-white hidden group-hover:block  py-1 px-3 inset-ring  hover:bg-green-600 h-14 rounded-xl">
                        <p class="w-full text-nowrap text-sm">Billy Joel</p>
                        <p class="w-full text-nowrap">Vienna</p>
                    </button>
                   
                 </div> 
             </div>
        </div>
    </div>

    <!-- video player -->
    <div class="w-160 mt-30 flex justify-end">
        <div class=" rotate-346 relative  w-120 h-84 p-1 button-back hover:gap-2  border-b-14  border-purple-500 rounded-4xl hover:p-1 hover:w-160 hover:transition-all duration-400 hover:cursor-pointer">
            <div class="w-full h-full hover:gap-2 group flex rounded-3xl bg-zinc-700   hover:transition-all duration-400 hover:cursor-pointer">
               <!-- video-player-in -->
                <div class="min-w-120 max-w-120  flex min-h-full max-h-full rounded-3xl p-1 button-back">   
                    <div class="h-full min-w-full rounded-3xl flex justify-between flex-col p-2 button-front">
                        <!-- top-player -->
                        <div class=" w-full h-[100%] rounded-3xl p-1 button-back ">   
                            <div class="h-full w-full rounded-3xl overflow-hidden ">
                                <img src={videoimage} alt="">
                            </div>
                        </div> 
                    </div>
                </div> 
                  <!-- video-setting-chooser -->
                 <div class=" group-hover:w-full flex group-hover:p-2 items-center justify-center group-hover:gap-4 flex-col">
                     <button class="w-18 h-18 rounded-full hover:cursor-crosshair text-white hidden group-hover:block py-1 px-3 inset-ring hover:bg-purple-600 ">
                        1
                    </button>
                    <button class="w-18 h-18 rounded-full hover:cursor-crosshair text-white hidden group-hover:block  py-1 px-3 inset-ring hover:bg-purple-600 ">
                        2
                    </button>
                    <button class="w-18 h-18 rounded-full hover:cursor-crosshair text-white hidden group-hover:block  py-1 px-3 inset-ring  hover:bg-purple-600 ">
                        3
                    </button>
                   
                 </div> 
             </div>
        </div>
    </div>
    <!-- photo viewer -->


  </div>