<template>
  <div class="flex flex-col min-h-screen bg-gray-50 text-gray-800">
    <main class="flex-1 max-w-5xl w-full mx-auto px-4 py-6">
      <div class="sticky top-0 z-20 flex flex-wrap items-center justify-between gap-3 bg-gray-50 pt-3 border-b border-gray-300 pb-3">
        <div class="flex flex-wrap gap-2">
          <p
            v-for="category in categories"
            :key="category"
            class="text-gray-600"
          >
            <span class="inline-block rounded-full bg-sky-100 px-3 py-1 text-sm">
              {{ category }}
            </span>
          </p>
        </div>
        <label class="relative w-full sm:w-56">
          <svg
            aria-hidden="true"
            class="pointer-events-none absolute left-3 top-1/2 h-4 w-4 -translate-y-1/2 text-gray-500"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            stroke-width="2"
          >
            <circle cx="11" cy="11" r="7" />
            <path stroke-linecap="round" d="m16 16 4 4" />
          </svg>
          <input
            type="search"
            aria-label="検索"
            placeholder="検索"
            class="w-full rounded-full border border-gray-300 bg-white py-2 pl-9 pr-3 text-sm"
          />
        </label>
      </div>
    </main>
  </div>
</template>

<script setup lang="ts">
const categories = ['研究', '雑談', '趣味', '就活', '悩み事']
</script>