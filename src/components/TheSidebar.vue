<template>
  <aside
    class="hidden xl:block w-64 max-h-screen overflow-auto fixed top-0 pt-12 z-20 bg-white"
  >
    <section class="py-2 border-b">
      <ul>
        <SidebarItem label="Home" icon="home" is-active />

        <SidebarItem label="Trending" icon="fire" />
        <SidebarItem label="Subscriptions" icon="collection" />
      </ul>
    </section>

    <section class="py-2 border-b">
      <ul>
        <SidebarItem label="Library" icon="duplicate" />
        <SidebarItem label="History" icon="clock" />
      </ul>
    </section>

    <section class="px-8 py-4 border-b font-medium leading-5">
      <span class="text-sm">Sign in to like vides, comment, and subscribe</span>
      <button
        class="flex items-center px-2 py-0.5 mt-3 text-sm text-blue-700 uppercase border border-blue-700 rounded"
      >
        <BaseIcon name="user" class="w-7 h-7 mr-2" />

        Sign In
      </button>
    </section>

    <section class="py-2 border-b">
      <div class="uppercase text-sm font-semibold px-6 py-2">
        Best of YouTube
      </div>
      <ul>
        <SidebarItem label="Music" icon="musicNote" />
        <SidebarItem label="Sports" icon="cup" />
        <SidebarItem label="Gaming" icon="puzzle" />
        <SidebarItem label="Movies" icon="movie" />
        <SidebarItem label="News" icon="news" />
        <SidebarItem label="Live" icon="live" />
        <SidebarItem label="360&deg; Video" icon="eye" />
      </ul>
    </section>

    <section class="py-2 border-b">
      <ul>
        <SidebarItem label="Browse channels" icon="plus" />
      </ul>
    </section>

    <section class="py-2 border-b">
      <div class="uppercase text-sm font-semibold px-6 py-2">
        More from YouTube
      </div>
      <ul>
        <SidebarItem label="Browse channels" icon="play" />
        <SidebarItem label="Live" icon="live" />
      </ul>
    </section>

    <section class="py-2 border-b">
      <ul>
        <SidebarItem label="Settings" icon="settings" />
        <SidebarItem label="Report history" icon="flag" />
        <SidebarItem label="Report history" icon="question" />
        <SidebarItem label="Send feedback" icon="message" />
      </ul>
    </section>

    <section class="px-6 py-5 text-xs font-semibold space-y-4">
      <div>
        <a href="#" class="mr-2">About</a>
        <a href="#" class="mr-2">Press</a>
        <a href="#" class="mr-2">Copyright</a>
        <a href="#" class="mr-2">Contact us</a>
        <a href="#" class="mr-2">Creators</a>
        <a href="#" class="mr-2">Advertise</a>
        <a href="#" class="mr-2">Developers</a>
      </div>
      <div>
        <a href="#" class="mr-2">Terms</a>
        <a href="#" class="mr-2">Privacy</a>
        <a href="#" class="mr-2">Policy &amp; Safety</a>
        <a href="#" class="mr-2">How YouTube works</a>
        <a href="#" class="mr-2">Test new features</a>
      </div>
      <div class="font-normal text-gray-500">&copy; 2023 Google LLC</div>
    </section>
  </aside>
</template>

<script>
import SidebarItem from "./SidebarItem.vue";
import BaseIcon from "./BaseIcon.vue";

export default {
  components: { SidebarItem, BaseIcon },
};
</script>
