<template>
  <Navbar />
  <main
    class="px-4 text-center text-gray-700 dark:text-gray-200"
    p="t-5.5rem"
  >
    <div class="grid grid-cols-12 container mx-auto">
      <div class="col-span-4">
        <Introduction />
      </div>
      <div class="col-span-8">
        <router-view />
      </div>
    </div>
    <Footer />
    <div class="mt-5 mx-auto text-center opacity-25 text-sm">
      [Home Layout]
    </div>
  </main>
</template>
