<template>
  <div class="border-t-8 border-green-500 min-h-screen flex flex-col items-center justify-center">
    <div>
    <header class="text-center py-8">
      <logo class="w-64 mx-auto"></logo>
      <!-- <g-image alt="A Bit Haywire" src="~/assets/images/logo.svg" class="w-64 mx-auto"/> -->
    </header>
    <main class="mb-8 -mt-24 border-8 border-green-500 sm:w-4/5 mx-auto max-w-4xl p-8 pt-16 bg-yellow-100">
      <slot/>
    </main>
    </div>
  </div>
</template>

<script>
import Logo from '../assets/svgs/Logo.svg'
export default {
  components: {
    Logo
  }
}
</script>

