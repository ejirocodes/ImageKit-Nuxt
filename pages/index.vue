<template>
  <div class="container">
    <client-only>
      <!-- <div>
        <ik-image
          path="/potriat_g-WKQi7tFiO15.jpg"
          :transformation="[
            { height: 500, width: 500, focus: 'face', format: 'webp' },
          ]"
          style="margin: 2rem"
        />
        <p>Face Smart cropping</p>
      </div> -->
      <div>
        <ik-image
          path="/mathilde-langevin-PM-ahoMuxhE-unsplash_o3JCZqZu8ibb.jpg"
          :transformation="[
            {
              height: 500,
              width: 500,
              focus: 'face',
              overlayText: 'Mathilde Langevin',
              overlayTextFontSize: 50,
              overlayTextColor: '2D5D62',
              overlayTextWidth: 300,
            },
          ]"
          :lqip="{ active: true, quality: 100, blur: 20 }"
          loading="lazy"
          style="margin: 2rem"
        />
        <!-- <p>Auto Smart cropping</p> -->
      </div>
      <!-- <ik-image
        path="/potriat_g-WKQi7tFiO15.jpg"
        :transformation="[
          {
            height: 400,
            width: 400,
            ooverlayText: 'ImageKit',
            overlayTextFontSize: 50,
            overlayTextColor: '000000',
          },
        ]"
      />

      <div>
        <ik-image
          path="/potriat_g-WKQi7tFiO15.jpg"
          :transformation="[{ height: 500, width: 500 }]"
          style="margin: 2rem"
        />
        <p>Default cropping</p>
      </div> -->

      <ik-image
        path="/default-image.jpg"
        loading="lazy"
        :transformation="[
          {
            overlayText: 'Image from ImageKit.io',
            overlayTextFontSize: 50,
            overlayTextColor: 'F7F7F7',
            overlayTextBackground: '1E212D',
            overlayTextPadding: '20_40_20_40',
            overlayTextWidth: 300,
            overlayRadius: 30,
            width: 700,
            height: 700,
          },
        ]"
        style="margin: 15rem"
      />

      <ik-image
        path="/mathilde-langevin-PM-ahoMuxhE-unsplash_o3JCZqZu8ibb.jpg"
        loading="lazy"
        :transformation="[
          {
            height: 600,
            width: 600,
            overlayImage:
              '/photo-1593642532400-2682810df593__1__n457ndv6CPXoL.jpg',
            overlayWidth: 200,
            overlayX: 0,
            overlayImageBorder: '10_000000',
            overlayImageQuality: 100,
          },
        ]"
        style="margin: 15rem"
      />

      <ik-image
        path="/photo-1593642532400-2682810df593__1__n457ndv6CPXoL.jpg"
        :lqip="{ active: true, quality: 20, blur: 10 }"
        :transformation="[
          {
            height: 600,
            width: 900,
            overlayText: 'Workspace setup',
            overlayTextFontSize: 50,
            overlayTextColor: 'FF005C',
            overlayTextBackground: 'F7F7F7',

            overlayTextWidth: 300,
            overlayRadius: 30,
          },
        ]"
        loading="lazy"
        height="600"
        width="900"
      />
      <!-- :transformation="[{ height: 600, width: 900 }]" -->
    </client-only>
  </div>
</template>

<script>
export default {
  data() {
    return {
      transformation: [{ height: 500, width: 500, focus: "face" }],
    };
  },
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 500vh;
  /* display: flex; */
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 160%;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
