<template>
    <b-container fluid>
        <b-row>
            <b-col class="col" cols="12" sm="4" md="3">
                <Bio />
            </b-col>
            <b-col class="col"  cols="12" sm="8" md="9">
                <div class="b-row project fixed" style="padding:15px 0 0 0; margin:0 0 0 0;">
                    <div class="tags" style="justify-content: space-between;">
                        <p class="biohead smallcaps"><span class="blue">Selection of work</span>
                        </p>
                        <!-- <div class="tags">
                            <p class="tag">design</p>
                            <p class="tag">development</p>
                            <p class="tag">all</p>
                        </div> -->
                    </div>
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
                hid: "og:url",
                property: "og:url",
                content: "https://byrthe.github.io/portfolio/",
            },
            {
                hid: "og:title",
                property: "og:title",
                content: "Byrthe Lemmens design and development portfolio",
            },
            {
                hid: "og:description",
                property: "og:description",
                content: "A small portfolio of Byrthe Lemmens of selected works in the graphic design and web development field.",
            },
            {
                hid: "og:image",
                property: "og:image",
                content: "/static/byrthelemmens-meta.jpg",
            },
            { property: "og:image:width", content: "1000" },
            { property: "og:image:height", content: "551" },
            {
                hid: 'Portfolio of designer and front-developer Byrthe Lemmens',
                name: 'Byrthe Lemmens - design and development',
                content: 'Portfolio of designer and front-end developer Byrthe Lemmens',
            },
        ],
    link: [{ rel: 'icon', type: 'image/x-icon', href: '/favi.png' }]
  },
}
</script>

<style>
</style>