<template>
    <section class="flex flex-col w-[1240px] mx-auto mb-16">
      <div class="mb-6">
          <h2  class="text-primary-black text-3xl font-semibold">Get inspiration for your next trip</h2>
      </div>
      <nexttripcard :nexttrips="nexttrips"/>
    </section>
</template>

<script>
import { ref } from 'vue';
import nexttripcard from './nexttripcard.vue'
export default {
  components: { nexttripcard },
  setup(){
        const nexttrips = ref([
            {
                /*i write img :'../../assets/imagename.png but it didn't show 
                even path correct and it shown without using bind so i use online link 
                vue bind on local link and add randum number every time !
                i traid to use impoet.meta.glob put it return glob in not a function error*/
                src:'https://s3-alpha-sig.figma.com/img/16a7/0720/741b1a33582ccbea66b737743968602d?Expires=1703462400&Signature=BdbyQFADvA51JX7~8CKgNkyL1PlPWwyl9n~BA5RJp~04mLGbeohrefELnczC31M3bFR0qhCUecfXR-uJMdGBIrxJEi4yuis65MMndE~UmIdGH8QImjU0j-U9snB3xRkqSJ5dRlzlIPBOJcWP1aBNqm1cR-xcaBPbz5b49trcRU3EljBnYIKHnhEmZ-XtlS3mFrrMc~DwYW4ZbMpq8xwatqXEIgczHedvM9mqOXjoRjqdet8ua44tDX0g9OOSLyKfC2y0ECaWDiMChWPrQ7~MIeMF6Cuu1NeptH2QfN~B7wt60rgZuwEvMVRHZbAx0ILP86wq0ydtmZqehde7KeQClA__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                pref:'Sydeny’s 10 most fashionable 5 star hotels',
                details:'Browse the fastest growing tourism sector in the heart of Australia tourism capital ....'
            },
            {
                src:'https://s3-alpha-sig.figma.com/img/6390/7bbf/e1389fbfd0626d0dbbf233f324dc4d3c?Expires=1704672000&Signature=SZm2CHGazoDAOfKeMzHB4GhhYdKpsNlwRUUY9jLZOcoYRhSb0xjo8CWenFmS56dM0~2b9qFq1gjH3e3zxuMZEDMwQFHD8XPtEEz6MsPYn8pTnfxS-ju8sfICwjkq1JTD1-0yALJIA98yL1HO0pDBf3Jh54etKt5Re53g9NIlOQ5oLDrqWmbo77aoSnlrAaQieeoQg5DjYDKf5pUBj8HuLFxqQOfyUgWtE~IRdJI7VCeR5NRG1Hl196lY41LBEDv15hNbmz4nOfuJkni8R2GbZmbrRSPrQzXTCI-PuBVYLchf5b026NxyDDbgS~q9y15~9I9VCS26QkyoaY5FEcCInw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                pref:'Top cities for Vegan Travellers',
                details:'Top sites where you do not have to worry about being a vegan. Our tourist guide is here...'
            },
            {
                src:'https://s3-alpha-sig.figma.com/img/5792/a4d6/add7dcaab1b06c4f605d4b8c5d5a707f?Expires=1704672000&Signature=Kn-WAt78NNaggKl-UZyCGCjodgwPjrLfxbCxmbxFZxYgw7t2wXCQ-G4HVdD5rCvB1DMx6fsKySmZUl8N8t5jPKeWMHvmWD3nFIRu1wzv6VJGyiQev7fCdPM9-XbmHEWlk6VEr5crCZE-XSOomROmk~C3Kv6qPFKQ7bDMaEZry7x0Ask9tZnq9A8B0Urp7OzfMzFcFA8KW6L-BqZviZA~iLS0NaHtyHChppI3lpO3V~I9XFDjsUW8OpFU1Fh1--PRFV91WyD7Zd4lOMxE7Qfr6T6kkpkUvcAQdiPpWjS81Mwk5aLPvImkyvWi-OeXWgfRnR-03SxGFohAwKcyIEgsTg__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                pref:'World’s top destinations during and post covid timeline',
                details:'Pandemic is still intact and will be here for a longer time. Here’s where your next destination...'
            },
        ])
        return { nexttrips }
    }
}
</script>