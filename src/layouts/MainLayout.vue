<template>
  <q-layout view="lHh Lpr lFf">
    <q-header
      style=" background-color: transparent !important;"
      elevated
      class="color:white !important;"
    >
      <q-toolbar>
        <q-toolbar-title>
          <q-img
            height="65px"
            width="45px"
            class="q-pt-sm q-pb-sm"
            src="../assets/google-stadia-logo.png"
          ></q-img>
        </q-toolbar-title>
        <q-space></q-space>
        <q-space></q-space>
        <q-btn
          style="background-image: linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%);

inline:1

linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%)"
          >About Stadia</q-btn
        >
        <q-btn
          class="q-ml-sm"
          style="background-image: linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%);

inline:1

linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%)"
          >Games</q-btn
        >
        <q-space></q-space>
        <q-space></q-space>

        <q-btn
          style="background-image: linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%);

inline:1
Best Match .vORvAb.hXyPqf
linear-gradient(90deg, rgb(248, 73, 27) 0%, rgb(241, 47, 63) 50%, rgb(220, 24, 96) 100%)"
          text-color="white"
          >Sign In</q-btn
        >
      </q-toolbar>
    </q-header>

    <!-- <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-grey-1"
    >
      <q-list>
        <q-item-label
          header
          class="text-grey-8"
        >
          Essential Links
        </q-item-label>
        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer> -->
    <VueScrollProgress>
      <q-page-container>
        <router-view />
      </q-page-container>
    </VueScrollProgress>
  </q-layout>
</template>

<script>
import EssentialLink from "components/EssentialLink.vue";

const linksData = [
  {
    title: "Docs",
    caption: "quasar.dev",
    icon: "school",
    link: "https://quasar.dev"
  },
  {
    title: "Github",
    caption: "github.com/quasarframework",
    icon: "code",
    link: "https://github.com/quasarframework"
  },
  {
    title: "Discord Chat Channel",
    caption: "chat.quasar.dev",
    icon: "chat",
    link: "https://chat.quasar.dev"
  },
  {
    title: "Forum",
    caption: "forum.quasar.dev",
    icon: "record_voice_over",
    link: "https://forum.quasar.dev"
  },
  {
    title: "Twitter",
    caption: "@quasarframework",
    icon: "rss_feed",
    link: "https://twitter.quasar.dev"
  },
  {
    title: "Facebook",
    caption: "@QuasarFramework",
    icon: "public",
    link: "https://facebook.quasar.dev"
  },
  {
    title: "Quasar Awesome",
    caption: "Community Quasar projects",
    icon: "favorite",
    link: "https://awesome.quasar.dev"
  }
];

export default {
  name: "MainLayout",
  components: { EssentialLink },
  data() {
    return {
      leftDrawerOpen: false,
      essentialLinks: linksData
    };
  }
};
</script>

<style lang="scss">
.q-layout__section--marginal {
}

/* play with some lines below */
#progress-container-el {
  /* background */
  background-color: #f4f4f4 !important;
}

#progress-el {
  /* progress bar */
  background-color: rgb(103, 8, 8) !important;
}
</style>
