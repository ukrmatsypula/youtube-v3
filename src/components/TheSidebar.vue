<template>
  <aside
    class="hidden xl:block w-64 max-h-screen overflow-auto fixed top-0 pt-16 z-20 bg-white"
  >
    <SidebarSection>
      <ul>
        <SidebarItem label="Home" icon="home" is-active />
        <SidebarItem label="Trending" icon="fire" />
        <SidebarItem label="Subscriptions" icon="collection" />
      </ul>
    </SidebarSection>

    <SidebarSection>
      <ul>
        <SidebarItem label="Library" icon="duplicate" />
        <SidebarItem label="History" icon="clock" />
      </ul>
    </SidebarSection>

    <SidebarSection class="px-8 py-4 border-b font-medium leading-5">
      <ul>
        <span class="text-sm"
          >Sign in to like vides, comment, and subscribe</span
        >
        <ButtonLogin
          class="focus:outline-none flex items-center px-2 py-0.5 mt-3 text-sm text-blue-700 uppercase border border-blue-700 rounded"
        />
      </ul>
    </SidebarSection>

    <SidebarSection class="px-8 py-4 border-b font-medium leading-5">
      <div class="uppercase text-sm font-semibold px-6 py-2">
        <SidebarSectionHeading title="Best of YouTube" />
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
    </SidebarSection>

    <SidebarSection class="px-8 py-4 border-b font-medium leading-5">
      <div class="uppercase text-sm font-semibold px-6 py-2">
        <SidebarSectionHeading title="More from YouTube" />
      </div>
      <ul>
        <SidebarItem label="Browse channels" icon="play" />
        <SidebarItem label="Live" icon="live" />
      </ul>
    </SidebarSection>

    <SidebarSection class="px-8 py-4 border-b font-medium leading-5">
      <ul>
        <SidebarItem label="Settings" icon="settings" />
        <SidebarItem label="Report history" icon="flag" />
        <SidebarItem label="Report history" icon="question" />
        <SidebarItem label="Send feedback" icon="message" />
      </ul>
    </SidebarSection>

    <SidebarSection class="px-6 py-5 text-xs font-semibold space-y-4">
      <TheFooter />
    </SidebarSection>
  </aside>
</template>

<script>
import SidebarItem from "./SidebarItem.vue";
import ButtonLogin from "./ButtonLogin.vue";
import SidebarSectionHeading from "./SidebarSectionHeading.vue";
import SidebarSection from "./SidebarSection.vue";
import TheFooter from "./TheFooter.vue";
export default {
  components: {
    SidebarItem,
    ButtonLogin,
    SidebarSectionHeading,
    SidebarSection,
    TheFooter,
  },
};
</script>
