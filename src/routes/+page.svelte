<script>
  import Nav from "$lib/components/Nav.svelte";
  import favicon from '$lib/assets/favicon.svg';
  import nodejs from "$lib/assets/nodejs-plain.svg"
  import illustator from "$lib/assets/illustrator-plain.svg"
  import postgrsql from "$lib/assets/postgresql-original.svg"
  import photoshop from "$lib/assets/photoshop-plain.svg"
  import figma from "$lib/assets/figma-original.svg"
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
    <!-- projects -->
     <div class="mt-40 w-160 flex flex-col gap-8">
       <div class=" h-50 bg-zinc-800 rounded-lg flex">2</div>
       <div class=" h-50 bg-green-700 rounded-lg flex">3</div>
       <div class=" h-50 bg-orange-700 rounded-lg flex">1</div>
       <div class=" h-50 bg-amber-950 rounded-lg flex">1</div>
     </div>

  </div>

