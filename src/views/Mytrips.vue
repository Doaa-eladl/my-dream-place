<template>
  <main class="bg-light-gray">
    <section class="w-[1030px] mx-auto">
        <h1 class="mb-7 pt-16 text-zinc-900 font-semibold text-3xl">My trips</h1>
        <div v-if="data.length==0" class="p-2 flex justify-center">
          <h2>No Trips yet</h2>
        </div>
        <tripcard :data="data"/>
    </section>
  <covedcheck class="pb-20 mt-52"/>
 </main>
</template>

<script>
import covedcheck from '@/components/repetativ component/covedcheck.vue'
import Tripcard from '@/components/Mytrips/tripcard.vue'
import { onMounted, ref } from 'vue'
import { usebooking } from '@/stores/booking'
export default {
  components: { covedcheck, Tripcard },
  setup(){
    const booking = usebooking()
    const data = ref([])
    onMounted(async()=>{
      data.value = await booking.getusertrips()
    })
    return { data }
  }
}
</script>