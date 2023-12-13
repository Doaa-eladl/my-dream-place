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
                src:'https://s3-alpha-sig.figma.com/img/6390/7bbf/e1389fbfd0626d0dbbf233f324dc4d3c?Expires=1703462400&Signature=m-lPhzj5p1OwrAl5OWbTP3EL76bBACUbWeV0pYF8u3kFWvSwp35BvgyBevKS3OBxmDcsjDqRKdOLgxC9rCGld-GmewmpcWaSEBeDHw4Taw-bN8fS6AWB7mlJa0Ke-FMeyzVzplEuOrHWvX0gIpc~YYjjElboeN9CPwVJCjHgc3WrhqvJAqkYuGPBJzRqbkhlJnI01UAD58dvkxOgcuPllR0~n7BlXB2M9uT3lLxtxW0nz0cHC~dOsmOj1wuXWTf3HacPEsgbrdg59u~k7ELUF3sdXOSubeZRUWiAqajKEG9WRjl-7FFMNSMIunw0KE9dtHklj8ODz5nMgJMgHGW9ZQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                pref:'Top cities for Vegan Travellers',
                details:'Top sites where you do not have to worry about being a vegan. Our tourist guide is here...'
            },
            {
                src:'https://s3-alpha-sig.figma.com/img/5792/a4d6/add7dcaab1b06c4f605d4b8c5d5a707f?Expires=1703462400&Signature=anH58EVkrd-DQvS1O5wU7fi263sBpNAUFW54n6~C0mblUA4E0hnMqRddqEfGHna0iOW5g7YRmG4dlxoILPyhViR1G1mjs0cq2eSH9F1mMyzXTJXU3Ai8dmXmseCd~u3yCqnbVesK2SFYbPx9AhVxzy6~EDaNfvEd6BuHRrpS5QpnkLzoMLFus-ApfFLehIgDsn4FZ3kZK9HVwNiMlTEBReI0i8S-4uPYSmLK-8hhG0HsWSYcDtzwYk6zaTP2uesHWN4zs~NoZErSVoZma0Gvh1gjwGkzKGs~i71GEWtN5OxBhDnbsIv-a4zuDCQYlmJJudBRn1egStVJlIiHwD~hsg__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                pref:'World’s top destinations during and post covid timeline',
                details:'Pandemic is still intact and will be here for a longer time. Here’s where your next destination...'
            },
        ])
        return { nexttrips }
    }
}
</script>