<script>
  import Mockup from './Mockup.svelte';
  export let label = "";
  export let type = "";
</script>

<div class="flex flex-col items-center group cursor-pointer w-full">
  <div class="w-full aspect-square bg-white rounded-[32px] border border-gray-100 shadow-[0_4px_24px_rgba(0,0,0,0.02)] flex items-center justify-center overflow-hidden relative transition-all duration-300 group-hover:-translate-y-1 group-hover:shadow-[0_12px_32px_rgba(0,0,0,0.04)]">
    <Mockup {type} />
  </div>
  <span class="mt-5 text-[13px] font-medium text-gray-400 group-hover:text-black transition-colors tracking-tight">{label}</span>
</div>
