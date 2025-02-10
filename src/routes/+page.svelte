<script>
  let { data } = $props()
  function refreshPage() {
    location.reload()
  }
</script>

<main
  class="relative flex flex-col items-center justify-center min-h-screen py-10"
>
  <h1
    class="pt-4 pb-8 bg-gradient-to-br dark:from-white from-black via-[#707070] to-[#ffffff] bg-clip-text text-center text-4xl font-medium tracking-tight text-transparent md:text-7xl"
  >
    Redis
  </h1>
  <div
    class="flex flex-col items-center w-full max-w-xl p-12 mx-auto rounded-lg shadow-xl dark:bg-white/10 bg-white/30 ring-1 ring-gray-900/5 backdrop-blur-lg"
  >
    <button
      onclick={refreshPage}
      class="mb-6 font-bold underline opacity-70 hover:opacity-100"
    >
      Refresh Page
    </button>
    <div class="text-5xl font-bold">
      {data?.pageVisits}
    </div>
  </div>
</main>
