<template>
    <section class="flex flex-col w-[1240px] mx-auto mb-16">
      <div class="mb-8">
          <h2  class="text-primary-black text-3xl	font-semibold mb-4">Popular hotels</h2>
      </div>
      <smallcard :data="hotels"/>
    </section>
  </template>
  
  <script>
  import { ref } from 'vue';
  import smallcard from '../repetativ component/smallcard.vue';
  export default {
      components:{smallcard},
      setup(){
        const hotels = ref([
              {
                /*i write img :'../../assets/imagename.png but it didn't show 
                even path correct and it shown without using bind so i use online link 
                vue bind on local link and add randum number every time !
                i traid to use impoet.meta.glob put it return glob in not a function error*/
                  img:'https://s3-alpha-sig.figma.com/img/bce4/6923/9fd793bdf7c58d302491fbb847a23511?Expires=1703462400&Signature=VZA~AQFiK~-Z92vTlU96akojQM5MP5IUzUE1mSrLXkUhtNyWpvThhIlbtsyYkkwnhXYA70BY7QyU0KXDnA9KAM9IiAMhWkn8UioDraGZM0-rAyRkDoi1YEIDfCGzA8mZzvKY0C1MIhM7hgJr8cGmpldxWej7wmJKVd9jhLupRSn3vQ5eD9qWu4~4gtQfUb6nGcLjmbZv4uKPwWkbXiPGroc14hYTxOmuUSQlgErIPhJSTKJ-tFZ79GjN8OgN82FkytDV4tWtyfZmCD48klyrBWDTifnCx2a57z5GKYYZuJWmkZbrwu5Qh2QUuUqLBbRStZE5MfOA8DC6fHq1iU0Gbw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Lakeside Motel Warefront',
                  numproperties:'2246 properties'
              },
              {
                  img:'https://s3-alpha-sig.figma.com/img/1dc8/bf3a/97f234423706967327b0a8fc1d82081f?Expires=1703462400&Signature=VKJam4Jl-IY4qnwNTdFssLYLRYem56w42UZZngG1cmltTp~dm54gNp1Uz74XOnTz7sB467b1CPMGKd1fS9PfaKt16n3eWAka76yADdvh3iV6vfFmma9942-oYmHF42s9nHqFk2msP8U8Rdtexd0LZiNecJmWR75fMGOORGbSjW4nARfE0uH~R3NsR9nF5K1ROBl1OxIRRHNuppy2Vewbfx31wYRNWy9S3zoJXBYOSnMFajZCDrP-UMChYacbF0vc0Qwzo2y-xkBNKVpaxsVe7rV1RcsvlbFhb4szzGZ6xh3~xerK8WlLOc8yBen701nUZJ0GRMYVFwhrUgrgn-VEWQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Recce Graham resort',
                  numproperties:'1278 properties'
              },
              {
                  img:'https://s3-alpha-sig.figma.com/img/009f/1ff6/45eb78fa3838f074fac563e6f14e5bb1?Expires=1703462400&Signature=Ryl-Uq7kw9NyLufv~K1mz3u2FMHhL7iLxTAzZW6zc13A5AFJJjNqYwIbpSNFRlIoOz1rB1AoxVcHV9ptwjcsRC95eCcPT0oeRNtR3VYCvy9SBC4bUpYrsEzv6HEI9JQssBcOpOk7HjB3RreEvIX98YpV6eNcEPtK0keQ3ukukdLMrhizPNC~MMzSVM100ICRvB5g56c5bUGcRUq7RinITxjkIOvIMiC5eEjPND3u160MvkRlWfPmi9YZe6ey94s0rd8Dsam8aUtOFFsCNBQRFoa4o0gq-WdsrmjZjkykrt2Q9L1HFuFcSB4NGBlo8xwXzPDsbvRHgb6aw6QaM~c2lw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Fireside Dinners',
                  numproperties:'480 properties'
              },
              {
                  img:'https://s3-alpha-sig.figma.com/img/b287/fb9d/73845d0e7dc924d9299658b292218a2d?Expires=1703462400&Signature=jf7YB5cOfrhF7UcK5GRilrJcZ-ZLdIpaM6YkHNMnZqkVrDlHs4Cl6rknOSaanrBnWjfZRrAwdlQjWhmZYZC53hBJwI9iMU~7Y1yn2gin~0kWuFUG0o7FPAFALlqKrIsU6Qb6bXIZMzSbvJ2U5H6Ulkjf3EV7GLtm6~-y35ij~pdOSPh-4Ror7mTcKxiOW81aPO14jdBdjJmXItq1zCa-Lnk6PwZygRCXSg2b461J0iTdv-WrnOQR04Yiw4FIoNZq~i4M4z5Dw5aTFM6yTdlRXP-RA8sdYZOOU2GAl7ShhLHKmXKixgM1sO0ZRLrBHqT-hpeQKLa-ocNna3LueaREMQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Oculous Inn Stay',
                  numproperties:'320 properties'
              },
          ])
        return { hotels }
      }
  }
  </script>