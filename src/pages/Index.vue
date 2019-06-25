<template>
  <Layout>
    <div class="sm:flex justify-between">
      <div class="sm:w-3/4">
        <p>Owen Bryce is a normal good-natured 10 year-old boy who likes robots and thinks all girls have cooties. One day, however, Owen will soon find out just how abnormal he really is. He'll find out when everything goes <strong class="text-700 italic">a bit haywire.</strong></p>
        <div class="py-8 sm:flex justify-between text-center">
          <div class="pb-4 sm:pb-0">
            <h3 class="font-bold leading-none"><a href="https://scottzirkel.com" class="text-green-400 hover:text-green-600">Scott Zirkel</a></h3>
            <h4>Writer</h4>
          </div>
          <div class="pb-4 sm:pb-0">
            <h3 class="font-bold leading-none">Courtney Huddleston</h3>
            <h4>Artist</h4>
          </div>
          <div class="pb-4 sm:pb-0">
            <h3 class="font-bold leading-none">Mike Garcia</h3>
            <h4>Colors</h4>
          </div>
        </div>
      </div>
      <div class="sm:ml-4">
        <div v-if="loading" class="flex flex-col item-center justify-center h-full">
          <a class="text-sm font-bold text-green-400" href="https://amzn.to/2X512kT">Buy on Amazon</a>
        </div>
        <iframe class="mx-auto" @load="loading = false" id="amazon" style="width:120px;height:240px;" marginwidth="0" marginheight="0" scrolling="no" frameborder="0" src="//ws-na.amazon-adsystem.com/widgets/q?ServiceVersion=20070822&OneJS=1&Operation=GetAdHtml&MarketPlace=US&source=ss&ref=as_ss_li_til&ad_type=product_link&tracking_id=sz1977-20&language=en_US&marketplace=amazon&region=US&placement=0977788350&asins=0977788350&linkId=ac929098a008fd1c37d4c4edbf40c936&show_border=false&link_opens_in_new_window=true"></iframe>
      </div>
    </div>
    <p class="text-xs pt-4">Copyright © 2007 - {{ (new Date()).getFullYear() }} Courtney Huddleston &amp; Viper Comics. All Rights Reserved.</p>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'A Bit Haywire'
  },
  data () {
    return {
      loading: true
    }
  }
}
</script>
