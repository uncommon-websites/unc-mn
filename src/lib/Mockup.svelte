<script>
  export let type = "brand";
</script>

<div class="w-full h-full flex items-center justify-center p-4">
  {#if type === "brand"}
    <!-- Billboard -->
    <div class="relative w-full h-full flex items-center justify-center">
      <!-- Pole -->
      <div class="absolute left-8 top-0 bottom-0 w-3 bg-gradient-to-r from-gray-300 to-gray-100 rounded-full shadow-inner z-10"></div>
      
      <!-- Brackets -->
      <div class="absolute left-8 top-[20%] w-6 h-3 bg-gray-300 rounded-r-md shadow-sm z-0"></div>
      <div class="absolute left-8 bottom-[20%] w-6 h-3 bg-gray-300 rounded-r-md shadow-sm z-0"></div>

      <!-- Frame -->
      <div class="relative ml-6 w-36 h-48 bg-white border-2 border-gray-200 shadow-xl flex flex-col overflow-hidden">
         <!-- Poster Content -->
         <div class="w-full h-full bg-gradient-to-br from-red-600 via-red-500 to-orange-400 p-4 flex flex-col justify-end">
            <div class="text-white/90 text-[8px] font-medium mb-1 opacity-80">⌘</div>
            <div class="text-white text-xl font-serif leading-[0.9] tracking-tight">
              Create<br>your<br>digital<br>mind
            </div>
         </div>
      </div>
    </div>

  {:else if type === "snippets"}
    <!-- Book -->
    <div class="relative w-full h-full flex items-end justify-center pb-6">
      <!-- Shelf -->
      <div class="absolute bottom-6 w-48 h-3 bg-[#a8a29e] rounded-sm shadow-lg z-0">
          <div class="w-full h-full bg-gradient-to-b from-transparent to-black/10"></div>
      </div>
      
      <!-- Book -->
      <div class="relative z-10 w-32 h-40 bg-[#e5e0d8] shadow-[-4px_0_10px_rgba(0,0,0,0.1)] flex flex-col p-4 transform -rotate-1 origin-bottom-left">
        <!-- Spine shadow effect -->
        <div class="absolute left-0 top-0 bottom-0 w-1 bg-gradient-to-r from-black/10 to-transparent"></div>
        
        <div class="text-[9px] text-gray-500 font-medium mb-2 tracking-wide">Delphi</div>
        <div class="text-base font-bold text-gray-800 mb-auto leading-tight">Snippets</div>
        
        <div class="text-[6px] text-gray-500 leading-relaxed text-right font-medium">
          Company<br>Growth<br>Ethos<br>Arc<br>YC
        </div>
      </div>
    </div>

  {:else if type === "website"}
    <!-- Tablet -->
    <div class="relative w-48 h-36 bg-gray-900 rounded-[18px] p-[6px] shadow-2xl transform rotate-[-1deg]">
      <!-- Screen -->
      <div class="w-full h-full bg-[#fffcf8] rounded-[12px] overflow-hidden flex flex-col relative">
        <!-- Browser Bar -->
        <div class="h-4 w-full bg-white border-b border-gray-100 flex items-center px-2 gap-1 z-10">
           <div class="w-1 h-1 rounded-full bg-gray-300"></div>
           <div class="w-1 h-1 rounded-full bg-gray-300"></div>
           <div class="w-1 h-1 rounded-full bg-gray-300"></div>
           <div class="mx-auto w-16 h-1.5 bg-gray-100 rounded-full"></div>
        </div>
        
        <!-- Web Content -->
        <div class="flex-1 overflow-hidden relative">
           <!-- Hero -->
           <div class="absolute top-0 left-0 right-0 h-24 bg-gradient-to-b from-[#fffcf8] to-white flex flex-col items-center pt-4">
              <div class="text-[6px] font-serif text-center leading-tight text-gray-800 mb-3">Your Mind.<br>Now on Demand.</div>
              <!-- Avatars row -->
              <div class="flex items-center justify-center gap-1 px-4 w-full">
                  <div class="h-8 flex-1 bg-red-900 rounded-sm"></div>
                  <div class="h-8 flex-1 bg-red-800 rounded-sm"></div>
                  <div class="h-8 flex-1 bg-red-700 rounded-sm"></div>
                  <div class="h-8 flex-1 bg-red-600 rounded-sm"></div>
                  <div class="h-8 flex-1 bg-red-500 rounded-sm"></div>
              </div>
           </div>
        </div>
      </div>
      <!-- Reflection -->
      <div class="absolute inset-0 bg-gradient-to-tr from-transparent via-white/5 to-transparent rounded-[18px] pointer-events-none"></div>
    </div>

  {:else if type === "ads"}
    <!-- Phone -->
    <div class="relative w-20 h-40 bg-gray-900 rounded-[16px] p-[3px] shadow-2xl transform rotate-[4deg]">
      <!-- Screen -->
      <div class="w-full h-full bg-red-950 rounded-[13px] overflow-hidden relative">
        <!-- Dynamic Island -->
        <div class="absolute top-1 left-1/2 -translate-x-1/2 w-5 h-1.5 bg-black rounded-full z-20"></div>
        
        <!-- Content -->
        <div class="w-full h-full bg-gradient-to-b from-red-900 via-red-700 to-red-900 flex flex-col items-center justify-center relative">
           <div class="w-12 h-12 rounded-full bg-red-500 blur-xl absolute top-1/4 opacity-50"></div>
           <div class="text-[5px] text-white/90 font-serif text-center relative z-10 leading-tight">Your Mind.<br>Now on Demand.</div>
           <div class="mt-4 w-8 h-2 bg-white/20 rounded-full"></div>
        </div>
      </div>
      <!-- Reflection -->
      <div class="absolute inset-0 bg-gradient-to-bl from-white/10 to-transparent rounded-[16px] pointer-events-none"></div>
    </div>

  {:else if type === "deck"}
    <!-- Monitor -->
    <div class="relative flex flex-col items-center justify-end h-full pb-4">
      <!-- Screen -->
      <div class="w-44 h-32 bg-gray-900 rounded-lg p-[2px] shadow-xl relative z-10">
         <div class="w-full h-full bg-white rounded-[6px] overflow-hidden relative">
            <!-- Slide Content -->
            <div class="absolute inset-0 bg-gradient-to-r from-orange-50 to-white flex items-center justify-center">
                <!-- Graphic -->
                <div class="w-32 h-16 bg-gradient-to-r from-orange-400 to-red-500 rounded opacity-90 blur-md absolute transform -skew-x-12"></div>
                <div class="relative z-10 text-[6px] font-serif text-white text-center drop-shadow-md">Create Your Digital Mind</div>
            </div>
         </div>
      </div>
      <!-- Stand -->
      <div class="w-8 h-10 bg-gradient-to-b from-gray-300 to-gray-200 -mt-4 z-0 shadow-inner"></div>
      <div class="w-20 h-1.5 bg-gray-300 rounded-full shadow-md"></div>
    </div>

  {/if}
</div>
