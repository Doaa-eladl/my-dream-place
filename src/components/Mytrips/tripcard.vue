<template>
  <div v-for="trip in props.data" :key="trip" class="bg-white w-[1030px] h-[240px] rounded	mx-auto p-5 flex justify-between mb-6">
    <div class="flex">
      <div class="mr-6">
        <img :src="trip.imgsrc" alt="hotel view" class="w-[285px] h-[200px] rounded	">
      </div>
      <div>
        <h2 class="text-zinc-900 text-xl font-medium mb-1.5">{{ trip.hotelname }}</h2>
        <div class="flex mb-8">
          <div class="flex mr-3">
            <img src="../../assets/star-s-fill 1.png" alt="full star rate" v-for="i in Number(trip.intrate)" :key="i">
            <img src="../../assets/star-s-fill 5.png" alt="half star rate" v-if="trip.doublerate>0">
          </div>
          <p class="font-normal text-sm	text-dark-gray">{{ trip.intrate }}<span v-if="trip.doublerate>0">.{{ trip.doublerate }}</span> ({{ trip.reviewnum }} Reviews)</p>
        </div>
        <div class="grid grid-rows-4 gap-y-2 font-normal text-sm text-dark-gray">
          <p class="text-red-500">Non refundable</p>
          <p>Check in: {{ new Date(booking.searchvalobj.checkindate)
        .toLocaleDateString("en-US", 
        {weekday: 'long', year: 'numeric', month: 'long', day: 'numeric'}) }}</p>
          <p>Check out: {{ new Date(booking.searchvalobj.checkoutdate)
        .toLocaleDateString("en-US", 
        {weekday: 'long', year: 'numeric', month: 'long', day: 'numeric'}) }}</p>
          <p>{{ Math.ceil(
            Math.abs(
            new Date(booking.searchvalobj.checkindate) - 
            new Date(booking.searchvalobj.checkoutdate))
            / (1000 * 60 * 60 * 24)) }}
         night stay</p>
        </div>
      </div>
    </div>
    <div class="flex flex-col justify-end items-end">
      <p class="text-zinc-900 text-xl font-medium mb-1.5">${{ Math.round(trip.price) }}</p>
      <p class="font-normal text-sm text-dark-gray mb-4">Includes taxes and fees</p>
      <router-link :to="{ name : 'hotel'}" class="btn">Includes taxes and fees</router-link>
    </div>
  </div>
</template>

<script>
import { usebooking } from '@/stores/booking'
export default {
  props:['data'],
  setup(props){
    const booking = usebooking()
    return { props , booking}
  }
}
</script>