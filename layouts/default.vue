<template>
    <b-container fluid>
        <b-row>
            <b-col class="col" cols="12" sm="4" md="3">
                <Bio />
            </b-col>
            <b-col class="col"  cols="12" sm="8" md="9">
                <div class="b-row project" style="padding:15px 0; margin:0 0 0 0;">
                    <p class="biohead smallcaps"><span class="blue">Selection of work</span>
                    </p>
                </div>
                <Nuxt />
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
export default{
    head: {
    title: 'Byrthe Lemmens portfolio',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      {
        hid: 'Portfolio of designer and front-developer Byrthe Lemmens',
        name: 'Byrthe Lemmens - design and development',
        content: 'Portfolio of designer and front-end developer Byrthe Lemmens'
      }
    ],
    link: [{ rel: 'icon', type: 'image/x-icon', href: '/favi.png' }]
  },
}
</script>

<style>
</style>