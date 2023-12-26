<template>
  <section class="flex flex-col w-[1240px] mx-auto mb-16">
    <div class="mb-8">
        <h2  class="text-primary-black text-3xl	font-semibold mb-4">Enjoy your dream vacation</h2>
        <p class="w-[610px] font-normal	text-base leading-6 tracking-wide">Plan and book our perfect trip with expert advice, travel tips, destination information and  inspiration from us</p>
    </div>
    <smallcard :data="dreamvacations"/>
  </section>
</template>

<script>
import { ref } from 'vue';
import smallcard from '../repetativ component/smallcard.vue';
export default {
    components:{smallcard},
    setup(){
        const dreamvacations = ref([
            {
                /*i write img :'../../assets/imagename.png but it didn't show 
                even path correct and it shown without using bind so i use online link 
                vue bind on local link and add randum number every time !
                i traid to use impoet.meta.glob put it return glob in not a function error*/
                img:"https://s3-alpha-sig.figma.com/img/69df/f285/a7422c6a633bfef99d433a171722b018?Expires=1703462400&Signature=lrN6WtxK3mR4YVzFtjl0yt9c1jxMj6Y6UEy1ETprLOweO5-r1KXi46g2HUicvzu4WxeMkO1GlqeUW2QxlPYaMO0dI8WUlpOt6peMOB1OOC0KuI~JkcjKnPUibgO-bTbNgXlW4CS57gjlak7Ziad799UXGNiDnp0KtXCtTAyG94yUqAKhcno1hz05b1Dbjm8LFHnrlk489ic5yabfXpFiEKIE2b7jT81uzRB6GrxmiuMmXInkeV77d~oO~C2VazVjajxwQGKe70Mw-qZ4uF3WIUtKAqI2ONHTetNYiOZa0zsb6AmSRaWY8bWms38phxjwl4ADcWy7vAOsWhfvTStDBQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4",
                name:'Australia',
                numproperties:'2246 properties'
            },
            {
                img:'https://s3-alpha-sig.figma.com/img/dd3d/907b/22070dc6b56b6e07bed3823c37b89f30?Expires=1704672000&Signature=Fv~-9JcXOJrOZCjW92LcvrwdwTdM0KmQFgTGpLYEj~fjMNCsNPFoGiMiuR9NTAeyZ7ba2wqioXepRsJ8R8GAX8CxV974AhZ2ejonfF4DfpkKxl6KLg8H7ac~hUsNM6aECmWlggZmCRyZggV03pclZfb5B9WJ11yTpJDSFQrdOHwt9iFoP0RM9jTht~2X86xxAMBhsN~Lwz7t-Fc4lnuO~v8cHL3VTWCBTM0qckZy~twniyzJRYizJE7zMEWcU3RsSfl4p4bDcIuY6gyAT8CJ9pTZ3Z6YhH1yAXJV1AuTdk0t0gjSpKfrUiBlOcoLNf95Jgn2ftudL1cgw61~ok8Piw__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                name:'Japan',
                numproperties:'1278 properties'
            },
            {
                img:'https://s3-alpha-sig.figma.com/img/1046/e3f1/52d5c751ccabb0e28e46ddd3404a7b92?Expires=1703462400&Signature=TMAaFA5mubLCh4egaTqER-~oAFFARiDiv4I~l10WaEWpT4lGxMWqmKt5Idx8Z~Iffw4bNXfplVuqF4UVX6qNjXB69~qbmahw-~jqfJy3CH-~nil0-MfRFqAyC9R6e9FG5pTdyCRxshgwqRox3DxWYlnA7~eAq3-6vxF2tfU3VU6QWn24x7tdBwv7VCl818ALRpU5qtN9OnWQV4hV2A65seNPDqrWKnqBKxq34TIUn1K5JGXhXy4WuxGYRvWKnCmzQvg5rsMlHXvYdhOVKBOuuaU23za1UzW2HqcSjgBn47ax~92Y4zHfZRh~852fd~tpl5~4mt5-~muNzKCFn4EiyQ__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                name:'New Zealand',
                numproperties:'480 properties'
            },
            {
                img:'https://s3-alpha-sig.figma.com/img/7982/f510/f73630bd7cb4fcd79d670100bd5cead7?Expires=1703462400&Signature=CzixTYRWAg~XESkZNRJtnDiz18Mrre86j2q0nzw4sSNYQwPxUPQdKP3bMDRkP7prQZEc44D6j5cP0~hvdQn02wYXxFcgu3fqGnOudSN~xcV0Mm9MkQBIqAWDYKKLo~GA6Qjej75Q6MF8763lJNptLCf6eGbFeZ4UpKEgpTn0Woun7L0YakI1fjNkI5pgjIVX-i43q~4l6eWcMIV-EOrDPRjEYfTWoaLEF8maSJxPk9glBM95ofPrUXTCDJdscGrL55KKcvKCD0mlycz-pQCB-iHCTqgX6rmDAwvnYCWPt3vGLGEDdenrdjdSknKb5cwBkLCRlyOn1x9DgjwC9GT8DA__&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4',
                name:'Greece',
                numproperties:'320 properties'
            },
        ])
        return { dreamvacations }
    }
}
</script>