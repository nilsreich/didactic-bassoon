# didactic-bassoon
EDVVV

<div v-scope="{ count: 0 }">
  {{ count }}
  <button @click="count++">inc</button>
</div>

<div v-scope="{ tab: 1 }" class="w-full h-96 bg-gray-50">
    <div class="flex">
        <button :class="[(tab===1) ? 'text-green-500 border-b border-green-500':'border-b ']"
            class="px-4 py-2" @click="tab=1">Tab 1</button>
        <button :class="[(tab===2) ? 'text-green-500 border-b border-green-500':'border-b ']"
            class="px-4 py-2" @click="tab=2">Tab 2</button>
        <button :class="[(tab===3) ? 'text-green-500 border-b border-green-500':'border-b ']"
            class="px-4 py-2" @click="tab=3">Tab 3</button>
        <div class="flex-1 border-b"></div>
    </div>
    <div class="p-2">
        <div v-if="tab===1">Auto</div>
        <div v-if="tab===2">Bus</div>
        <div v-if="tab===3">Hase</div>
    </div>
</div>