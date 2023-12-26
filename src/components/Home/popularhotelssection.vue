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
                  img:'https://s3-alpha-sig.figma.com/img/bce4/6923/9fd793bdf7c58d302491fbb847a23511?Expires=1704672000&Signature=B~vzoWs7ILPFiX~xyyEwi2NooSb14vFSIF8Ado8yLwLdpFmgxhRBlcHumP10dUaET5sshMMFy5RnipfVTSVmteAgUkAdeWqrLonTsKVFFAin6T5ZHTqhnvbZEj3h4KQV8wkksbmQpw6yrFzcKV4byu3Y2ktpckm0GzcgSQWlkW-vstBOLoEQtVSx8cMn6Y7itIE8MJxHrSq6POVMRDoZibns1qpU0h6mcBiGxkQdOBdxqoXBvL8iNt6yAhqc6oR2ksWM~LIkWbTb12TWWxdFh4VBEyyKu3Wa3~uRwG~GDM86Zv8QxQEErhRhOdQKqGdb3rXmhEHU-5lOHWDszX1ReA__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Lakeside Motel Warefront',
                  numproperties:'2246 properties'
              },
              {
                  img:'https://s3-alpha-sig.figma.com/img/1dc8/bf3a/97f234423706967327b0a8fc1d82081f?Expires=1704672000&Signature=DayrjGqV7sxDyppaCunx8utRVSeAI9MnCsZzBJJXYD9Ip1k3xM3P8wEy-APY8ufobv6j8vWPOndYSio0jxvjMYx6mnWef7Y9p4PskpkFK9qRPT13jOvTQnI6diPCAxeb4ysiMYhunFv1nO1wc~swg39v7dGhDnqioCBrCynaJjoDCMuj9UKepFfmgVIPy4FaMiNdybx08dvnegW-j-RgVWFILNosI9q4Yy1IGg8MupUkV8nTyAlyxL~VjlMEpHxpHF-KHVkel-0hZDP7DuK1YfOsRU8jfAfb4wtp44cMiwVuYANoE8Uj5QsziQv03V9UM2C4UeOMrr48bD3Zkh5USA__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Recce Graham resort',
                  numproperties:'1278 properties'
              },
              {
                  img:'https://s3-alpha-sig.figma.com/img/009f/1ff6/45eb78fa3838f074fac563e6f14e5bb1?Expires=1704672000&Signature=l2yVgJ0-L4jJ2AICZB0LAtPYywmBlXbgf04~42UPk5rfl5QvBA36TZFXwTu5-aCI1HAzY7wyR~VhCgOivZGDq-1oxhVo1acdSlcsXbtuJffiQMi4fsKaEKpQ4X1r2wfymvRgDOdsMe7bKiTAKj-pmVpi7o210D329QPeTMpoCIsdAqebsUvPDRc09hSIMim-a5wrne6tdH3FEo2ic9MhkKfBCCH1Kok7FQPFtSmpIDV4S7U06TcGtOZ~6cDa4o6g8VvI2AS7OyI2KM~o2k67jNroITLTc2OwrdieW8ETDbCEGKSyKgwr~a31Z81vsgh3KcUU7tQaDpy~fl-GcYgVag__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Fireside Dinners',
                  numproperties:'480 properties'
              },
              {
                  img:'https://s3-alpha-sig.figma.com/img/b287/fb9d/73845d0e7dc924d9299658b292218a2d?Expires=1704672000&Signature=WrcCDkw1pvmVMt-A1kPuN0K4AxP7RE3icLA6WzDANqVdqvF-YTDZlrKu3aOSxNoHwUaL6HTzv22irnLeZENMfHCdxotaNSmvID7SCv1x-h6y7m~-nElTwtAezAGLliQCGZ84CvY92TRWQjKd3TO5fSgnQ0wnQAn~GtXt1B35Wg~Oq0lu2oHxiLXZwhx~AbiCzszDj9p0PAo-pMjDv6WTf-dFf2heBuiSFlxJkGXFRD4uqvGFdMSmXTTDqrqsQsZAb~r7aI3h8fDW-FFpzB5FwWWwgwLwMav4y7ba7NMmACfea5WaQmUIEjsIMZmI72c7x7RxVqt8Vx9NrtC57k16Uw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                  name:'Oculous Inn Stay',
                  numproperties:'320 properties'
              },
          ])
        return { hotels }
      }
  }
  </script>