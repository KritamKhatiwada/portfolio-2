<script>
  import Nav from "$lib/components/Nav.svelte";
  import favicon from '$lib/assets/favicon.svg';
  import nodejs from "$lib/assets/nodejs-plain.svg"
  import illustator from "$lib/assets/illustrator-plain.svg"
  import postgrsql from "$lib/assets/postgresql-original.svg"
  import photoshop from "$lib/assets/photoshop-plain.svg"
  import figma from "$lib/assets/figma-original.svg"
  import arrow from "$lib/assets/arrow-up-right-svgrepo-com.svg"
  import javascriptlogo from "$lib/assets/javascript-plain.svg"
  import csslogo from "$lib/assets/css3-plain.svg"
  import p1 from "$lib/assets/amazon-phone-mockup.png"
  // import htmllogo from "$lib/assets/css3-plain.svg"
</script>

<div class="flex flex-col py-6  text-center w-screen bg-white h-auto items-center ">
    <Nav/>
    <!-- headline -->
    <div class="mt-40">
        <p class="text-4xl">Hello! I am <span class="font-bold text-4xl">Kritam Khatiwada</span></p>
        <p class="text-xl mt-4">I am a Web Developer & UI/UX Designer</p>
        <p class=text-xl>From Morang, Nepal.</p>
    </div>
    <!-- tags -->
    <div class="mt-6 gap-4 w-160 flex flex-wrap justify-center">
      <div class="h-10 w-auto p-[1px]  flex rounded-full  button-back  justify-center items-center ">  <button class="w-full h-full gap-2 p-3 flex justify-center items-center text-black text-sm font-semibold  rounded-full bg-white hover:cursor-pointer"> <img src="{favicon}" alt="S" srcset="" height="16px" width="16px"> SVELTEKIT</button></div>
      <div class="h-10 w-auto p-[1px]  flex rounded-full  button-back  justify-center items-center ">  <button class="w-full h-full gap-2 p-3 flex justify-center items-center text-black text-sm font-semibold  rounded-full bg-white hover:cursor-pointer"> <img src="{nodejs}" alt="js" srcset="" height="16px" width="16px"> NODEJS</button></div>
      <div class="h-10 w-auto p-[1px]  flex rounded-full  button-back  justify-center items-center ">  <button class="w-full h-full gap-2 p-3 flex justify-center items-center text-black text-sm font-semibold  rounded-full bg-white hover:cursor-pointer"> <img src="{postgrsql}" alt="E" srcset="" height="16px" width="16px"> POSTGRESQL</button></div>
      <div class="h-10 w-auto p-[1px]  flex rounded-full  button-back  justify-center items-center ">  <button class="w-full h-full gap-2 p-3 flex justify-center items-center text-black text-sm font-semibold  rounded-full bg-white hover:cursor-pointer"> <img src="{illustator}" alt="Ai" srcset="" height="16px" width="16px"> ILLUSTRATOR</button></div>
      <div class="h-10 w-auto p-[1px]  flex rounded-full  button-back  justify-center items-center ">  <button class="w-full h-full gap-2 p-3 flex justify-center items-center text-black text-sm font-semibold  rounded-full bg-white hover:cursor-pointer"> <img src="{photoshop}" alt="Ps" srcset="" height="16px" width="16px"> PHOTOSHOP</button></div>
      <div class="h-10 w-auto p-[1px]  flex rounded-full  button-back  justify-center items-center ">  <button class="w-full h-full gap-2 p-3 flex justify-center items-center text-black text-sm font-semibold  rounded-full bg-white hover:cursor-pointer"> <img src="{figma}" alt="F" srcset="" height="16px" width="16px"> FIGMA</button></div>
      
    </div>
    <p class="mt-60 w-160 text-left font-bold text-4xl">PROJECTS</p>
    <!-- projects -->
    <div class="mt-8 w-160 flex flex-col gap-8">
      <!-- project 1 -->
      <div class=" h-50 w-full justify-between p-8 bg-zinc-800 rounded-lg flex">
        
          <img src="{p1}" alt="">
        <div class="flex flex-col w-120 items-end justify-between">
          <div class="text-4xl text-white font-bold">E-Commerce Website</div>
          <div class="flex gap-8">
            <!-- techstack -->
             <div class="flex gap-4">
               <img src="{javascriptlogo}" alt="" height="36x" width="36px">
               <img src="{csslogo}" alt="" height="36x" width="36px">
               <!-- <img src="{htmllogo}" alt="" height="36x" width="36px"> -->
             </div>
            <!-- button -->
            <div class=" w-auto p-1 bg-zinc-300 rounded-full flex items-center ">
              <div class="h-10 w-36 p-[1px]  flex rounded-full  button-back  justify-between items-center ">
                  <button class="w-full h-full text-zinc-700  p-2 flex  items-center text-sm  rounded-full bg-white hover:cursor-pointer"> 
                    <div class="w-7 h-7 rounded-full flex justify-center mr-5 bg-zinc-800">
                      <img src="{arrow}" alt="F" srcset="" height="16px" width="16px">
                    </div> 
                    <span class="">See More</span>
                  </button>
                </div>
            </div>
            
          </div>
        </div>
       </div>
       <!-- project 2 -->
      <div class=" h-50 justify-between p-8 bg-green-800 rounded-lg flex">
        <div class="h-full w-30 bg-amber-800 rounded-7xl"></div>
        <div class="flex flex-col w-[70%] items-end justify-between">
          <div class="text-4xl text-white font-bold">Memo Notepad</div>
          <div class="flex gap-8">
            <!-- techstack -->
             <div class="flex gap-4">
               <img src="" alt="">
               <img src="" alt="">
             </div>
            <!-- button -->
            <div class=" w-auto p-1 bg-zinc-300 rounded-full flex items-center ">
              <div class="h-10 w-36 p-[1px]  flex rounded-full  button-back  justify-between items-center ">
                  <button class="w-full h-full text-zinc-700  p-2 flex  items-center text-sm  rounded-full bg-white hover:cursor-pointer"> 
                    <div class="w-7 h-7 rounded-full flex justify-center mr-5 bg-zinc-800">
                      <img src="{arrow}" alt="F" srcset="" height="16px" width="16px">
                    </div> 
                    <span class="">See More</span>
                  </button>
                </div>
            </div>
            
          </div>
        </div>
       </div>
       <!-- project 3 -->
      <div class=" h-50 justify-between p-8 bg-orange-700 rounded-lg flex">
        <div class="h-full w-30 bg-white rounded-7xl"></div>
        <div class="flex flex-col w-[70%] items-end justify-between">
          <div class="text-4xl text-white font-bold"> NepaFair</div>
          <div class="flex gap-8">
            <!-- techstack -->
             <div class="flex gap-4">
               <img src="" alt="">
               <img src="" alt="">
             </div>
            <!-- button -->
            <div class=" w-auto p-1 bg-zinc-300 rounded-full flex items-center ">
              <div class="h-10 w-36 p-[1px]  flex rounded-full  button-back  justify-between items-center ">
                  <button class="w-full h-full text-zinc-700  p-2 flex  items-center text-sm  rounded-full bg-white hover:cursor-pointer"> 
                    <div class="w-7 h-7 rounded-full flex justify-center mr-5 bg-zinc-800">
                      <img src="{arrow}" alt="F" srcset="" height="16px" width="16px">
                    </div> 
                    <span class="">See More</span>
                  </button>
                </div>
            </div>
            
          </div>
        </div>
      </div>
      <!-- project-4 -->
      <div class=" h-50 justify-between p-8 bg-amber-950 rounded-lg flex">
        <div class="h-full w-30 bg-yellow-600 rounded-7xl"></div>
        <div class="flex flex-col w-[70%] items-end justify-between">
          <div class="text-4xl text-white font-bold">Metro Cleaner Website</div>
          <div class="flex gap-8">
            <!-- techstack -->
             <div class="flex gap-4">
               <img src="" alt="">
               <img src="" alt="">
             </div>
            <!-- button -->
            <div class=" w-auto p-1 bg-zinc-300 rounded-full flex items-center ">
              <div class="h-10 w-36 p-[1px]  flex rounded-full  button-back  justify-between items-center ">
                  <button class="w-full h-full text-zinc-700  p-2 flex  items-center text-sm  rounded-full bg-white hover:cursor-pointer"> 
                    <div class="w-7 h-7 rounded-full flex justify-center mr-5 bg-zinc-800">
                      <img src="{arrow}" alt="F" srcset="" height="16px" width="16px">
                    </div> 
                    <span class="">See More</span>
                  </button>
                </div>
            </div>
            
          </div>
        </div>
       </div>
    </div>
</div>

